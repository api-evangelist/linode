---
name: linode-estimate-cost-before-provisioning
description: Price a stack on Akamai Cloud (Linode) before spending anything, using the provider's unauthenticated price-book endpoints.
api: linode:linode-regions-api
openapi: openapi/linode-regions-api-openapi.yml
operations:
  - getRegions
  - getRegion
  - getLinodeTypes
generated: '2026-09-17'
method: generated
source: live probe of https://api.linode.com/v4/linode/types plus openapi/linode-regions-api-openapi.yml
---

# Estimate cost before you provision

Linode publishes its price book as an **unauthenticated API**. You can cost an entire stack without a
token, an account, or a sales conversation — which makes this the safest first call an agent can make
against this provider, and the one to make before any billable write.

## The price-book endpoints

All of these answer `200` with no `Authorization` header:

    GET /v4/linode/types             compute plans (75 types, 2026-09-17)
    GET /v4/volumes/types            Block Storage
    GET /v4/nodebalancers/types      load balancers
    GET /v4/lke/types                LKE control-plane tiers
    GET /v4/object-storage/types     Object Storage
    GET /v4/databases/types          Managed Databases
    GET /v4/network-transfer/prices  transfer overage
    GET /v4/regions                  regions and their capabilities

## Reading a compute plan correctly

Each entry in `/linode/types` looks like this:

```json
{
  "id": "g6-nanode-1",
  "label": "Nanode 1GB",
  "price":  { "hourly": 0.0075, "monthly": 5.0 },
  "region_prices": [ { "id": "id-cgk", "hourly": 0.009, "monthly": 6.0 } ],
  "addons": { "backups": { "price": { "hourly": 0.003, "monthly": 2.0 },
                           "region_prices": [ ... ] } },
  "memory": 1024, "disk": 25600, "transfer": 1000, "vcpus": 1, "gpus": 0,
  "class": "nanode"
}
```

Three things trip up a naive estimate:

1. **`region_prices` overrides `price`.** Jakarta (`id-cgk`) and São Paulo (`br-gru`) cost more than
   the base rate on every plan. Always look up the target region in `region_prices` first and only
   fall back to `price` when it is absent.
2. **Backups are priced per plan, in `addons`, and are not included.** They are also the only reversal
   path this provider has for a destroyed instance, so an estimate that omits them is not comparable
   to one that includes them.
3. **Some classes return `0`.** The GPU class returns a `0` base monthly price on the public catalog;
   its real cost is region- or entitlement-driven. Do not report `$0` — report that the public
   catalog does not price it and that the figure must come from Akamai.

## Check stock, not just price

    GET /v4/regions                  -> getRegions
    GET /v4/regions/{regionId}       -> getRegion

A plan being listed does not mean it is available where you want it. Confirm the region carries the
capability you need (`Linodes`, `Kubernetes`, `Object Storage`, `GPU Linodes`) before quoting.

## Billing model

Hourly, capped at the monthly rate. An instance billed at `$0.0075/hr` never exceeds `$5.00` in a
month. Shutting an instance down does **not** stop billing — only deleting it does.

## Then hand off

Once the estimate is agreed, the provisioning steps are in
`skills/linode-deploy-compute-instance.md` and `skills/linode-provision-lke-cluster.md`. Both write
surfaces are billable and neither has an idempotency key.
