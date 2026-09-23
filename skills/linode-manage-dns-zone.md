---
name: linode-manage-dns-zone
description: Create a DNS zone on Linode's nameservers and manage its records, with the deletion hazards stated up front.
api: linode:linode-domains-api
openapi: openapi/linode-domains-api-openapi.yml
operations:
  - getDomains
  - createDomain
  - getDomain
  - updateDomain
  - deleteDomain
  - getDomainRecords
  - createDomainRecord
generated: '2026-09-17'
method: generated
source: openapi/linode-domains-api-openapi.yml plus https://techdocs.akamai.com/linode-api/reference/get-started
---

# Manage a DNS zone on Linode

Base URL `https://api.linode.com/v4`, `Authorization: Bearer <token>`. DNS hosting is free with a
Linode account, which is why this surface is a common first automation — and why getting it wrong is
expensive: a deleted zone takes the site down and there is no recycle bin.

## Stop conditions

* **`deleteDomain` is immediate and permanent.** There is no restore operation, no soft delete and no
  documented grace period. Deleting a zone removes every record in it.
* **No idempotency key.** A retried `createDomainRecord` after a timeout creates a duplicate record.
  Read `getDomainRecords` and match on `type` + `name` + `target` before retrying.
* Export the zone before any destructive change: `GET /domains/{domainId}/zone-file` in the full
  contract returns the zone file as text. Store it somewhere outside this API.

## 1. Find or create the zone

    GET  /domains                 -> getDomains
    POST /domains                 -> createDomain

For a `master` zone send `domain`, `type: master` and `soa_email`. For a `slave` zone send
`master_ips[]`. The returned `id` is a bare integer.

Filter the collection with a JSON `X-Filter` header, for example
`X-Filter: {"domain": "example.com"}` — not with a query parameter.

## 2. Read and add records

    GET  /domains/{domainId}/records   -> getDomainRecords
    POST /domains/{domainId}/records   -> createDomainRecord

Record types available: `A`, `AAAA`, `NS`, `MX`, `CNAME`, `TXT`, `SRV`, `PTR`, `CAA`. Send `type`,
`name` (the subdomain, empty string for the apex), `target`, and `ttl_sec`.

A `ttl_sec` of `0` means "use the default", not "no caching". Set it explicitly before a planned
cutover so the old value expires when you expect.

## 3. Update the zone

    PUT /domains/{domainId}       -> updateDomain

Changing `soa_email`, `refresh_sec`, `retry_sec`, `expire_sec` or `status` on the zone does not touch
the records.

## Checking the change landed

The Linode API confirms it accepted the record; it does not tell you the change has propagated. Verify
against Linode's nameservers directly (`ns1.linode.com` ... `ns5.linode.com`) before reporting success.

## Errors and limits

`{"errors": [{"field": "...", "reason": "..."}]}` — vendor envelope, not RFC 9457. A `400` on a record
create usually names the offending field; a `404` means the zone id is wrong *or* belongs to another
account. Default limits: 200/min on paginated GETs, 1600/min otherwise, `429` with `Retry-After`.
