---
name: linode-provision-lke-cluster
description: Stand up a Linode Kubernetes Engine cluster, add a node pool, retrieve the kubeconfig, and tear it down safely.
api: linode:linode-linode-kubernetes-engine-lke-api
openapi: openapi/linode-linode-kubernetes-engine-lke-api-openapi.yml
operations:
  - getLKEVersions
  - getLKEClusters
  - createLKECluster
  - getLKECluster
  - updateLKECluster
  - getLKENodePools
  - createLKENodePool
  - getLKEClusterKubeconfig
  - deleteLKECluster
generated: '2026-09-17'
method: generated
source: openapi/linode-linode-kubernetes-engine-lke-api-openapi.yml plus https://techdocs.akamai.com/linode-api/reference/get-started
---

# Provision an LKE cluster

Base URL `https://api.linode.com/v4`, `Authorization: Bearer <token>`. The LKE control plane is free
on the standard tier; you pay for the nodes in the pools you create, priced as ordinary compute
instances from `/linode/types`.

## 1. Choose a Kubernetes version

    GET /lke/versions        -> getLKEVersions

Never hard-code a version. The list changes and an unsupported version is rejected at create time
with a `400` naming the `k8s_version` field.

## 2. Create the cluster

    POST /lke/clusters       -> createLKECluster

Send `region`, `k8s_version`, `label`, and `node_pools[]` with a `type` and `count` per pool. The
nodes are billable from the moment they provision.

**No idempotency key exists.** A retried `createLKECluster` creates a second cluster and a second set
of billable nodes. On a timeout, call `getLKEClusters` and match on `label` before retrying.

## 3. Wait, then read the kubeconfig

    GET /lke/clusters/{clusterId}             -> getLKECluster
    GET /lke/clusters/{clusterId}/kubeconfig  -> getLKEClusterKubeconfig

The kubeconfig is **not available immediately**. Akamai's own operation description says it often
takes 2-5 minutes after cluster creation before the file is ready, so poll rather than treating the
first failure as fatal.

The response is `{"kubeconfig": "<base64>"}` and it is a **cluster-admin credential**. Do not log it, do
not echo it into a transcript, and do not write it anywhere an agent transcript is retained. Akamai's
own MCP server refuses to return it for exactly this reason.

## 4. Scale

    GET  /lke/clusters/{clusterId}/pools      -> getLKENodePools
    POST /lke/clusters/{clusterId}/pools      -> createLKENodePool
    PUT  /lke/clusters/{clusterId}            -> updateLKECluster

Adding a pool adds billable nodes. Recycling or resizing a pool replaces nodes; anything stored on a
node's local disk is lost. Persistent data belongs on a Block Storage volume or Object Storage.

## 5. Delete

    DELETE /lke/clusters/{clusterId}          -> deleteLKECluster

Deleting the cluster deletes its nodes. **Volumes provisioned by the Linode CSI driver are not
necessarily deleted with it** — check `/volumes` afterwards, or you keep paying for orphaned Block
Storage. There is no undelete for the cluster.

## Errors and limits

Vendor error envelope: `{"errors": [{"field": "...", "reason": "..."}]}`. Not RFC 9457. Match on the
HTTP status plus `reason` prose.

Default limits: 200 requests/minute on paginated GET collections, 1600/minute on everything else,
`429` on exhaustion with `Retry-After` and `X-RateLimit-*` headers. Collections paginate with
`page`/`page_size` (1-based, 25-500, default 100) and filter through a JSON `X-Filter` header.
