---
name: linode-deploy-compute-instance
description: Deploy, verify, resize and retire a Linode compute instance on Akamai Cloud, with the region and plan chosen from the live catalog rather than guessed.
api: linode:linode-linode-instances-api
openapi: openapi/linode-linode-instances-api-openapi.yml
operations:
  - getLinodeTypes
  - getLinodeInstances
  - createLinodeInstance
  - getLinodeInstance
  - bootLinodeInstance
  - rebootLinodeInstance
  - shutdownLinodeInstance
  - resizeLinodeInstance
  - deleteLinodeInstance
generated: '2026-09-17'
method: generated
source: openapi/linode-linode-instances-api-openapi.yml plus https://techdocs.akamai.com/linode-api/reference/get-started
---

# Deploy a compute instance on Akamai Cloud (Linode)

Base URL `https://api.linode.com/v4`. Every call carries `Authorization: Bearer <token>`, where the
token is a Linode personal access token or an OAuth access token. Creating and deleting instances are
**billable, irreversible actions** — read the stop conditions below before the first write.

## Before you write anything

**There is no idempotency key in this API.** No operation accepts `Idempotency-Key`, and the contract
declares none. If `createLinodeInstance` times out and you retry it, you get a second running instance
and a second bill. Treat every write as at-most-once: on a timeout, call `getLinodeInstances` and
filter by the `label` you sent before retrying.

**There is no undo for `deleteLinodeInstance`.** Deletion is immediate and permanent; the API has no
restore-deleted-instance operation and documents no grace period. The only recovery path is a restore
from a backup taken *before* the delete (`post-restore-backup` in the full first-party contract; the
split instances spec here carries only `getBackups`), and only if the paid Backups service was already
enabled on that instance. Automated backups are kept no longer than 14 days.

## 1. Pick a plan and a region from the catalog, not from memory

    GET /linode/types        -> getLinodeTypes
    GET /regions             -> (Regions API, getRegions)

Both are public: they answer with no credential at all. Each type carries `price.hourly`,
`price.monthly`, `region_prices[]` (some regions cost more), `vcpus`, `memory`, `disk`, `transfer` and
`addons.backups.price`. Read the price from here rather than from a pricing page — this endpoint is
the provider's own price book and it is the source its MCP server uses to estimate cost.

Check that the plan is actually in stock in the region you want before you try to create in it.

## 2. Create the instance

    POST /linode/instances   -> createLinodeInstance

Send `region`, `type`, a `label` you can search on later, and either `root_pass` or `authorized_keys`.
Record the returned `id` immediately; it is a bare integer and nothing else in the response identifies
it as an instance.

Rate limit: **20 requests per 15 seconds** on this operation specifically, not the 1600/minute default.

The instance returns with `status: provisioning`. Poll `getLinodeInstance` until `status` reaches
`running` before doing anything else with it.

## 3. Operate it

    GET    /linode/instances/{linodeId}          -> getLinodeInstance
    POST   /linode/instances/{linodeId}/boot     -> bootLinodeInstance
    POST   /linode/instances/{linodeId}/reboot   -> rebootLinodeInstance
    POST   /linode/instances/{linodeId}/shutdown -> shutdownLinodeInstance
    POST   /linode/instances/{linodeId}/resize   -> resizeLinodeInstance

`resizeLinodeInstance` reboots the instance and can take a long time on large disks. It is not
reversible on its own — resizing back down is a second resize, and a disk that has grown may not fit
the smaller plan.

## 4. Retire it

    DELETE /linode/instances/{linodeId}          -> deleteLinodeInstance

Shutting an instance down does **not** stop billing; only deleting it does. Confirm with a human
before calling this, and confirm the `id` by reading `label` back from `getLinodeInstance` first —
the id is an integer with no type prefix and a wrong one deletes the wrong machine.

## Errors and limits

Errors come back as `{"errors": [{"field": "...", "reason": "..."}]}` — not RFC 9457 problem+json.
There are no stable error codes; match on `reason` text and on the HTTP status.

* `400` — read `errors[].field`, fix that field, retry.
* `401` — invalid or expired token. Linode tokens carry a fixed expiry set at creation.
* `403` — the token lacks the scope, or the user lacks the IAM permission, for this operation.
* `404` — the instance does not exist *or* is outside this account. Linode does not distinguish.
* `429` — wait for `Retry-After` (seconds) or `X-RateLimit-Reset` (UTC epoch seconds).

Paginated collections return `{data, page, pages, results}`; `page` starts at 1 and `page_size`
accepts 25-500, default 100. Filter collections with a JSON document in the `X-Filter` request
header, not with query parameters.
