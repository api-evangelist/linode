# linode (linode)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Linode is a cloud hosting provider offering virtual private servers, managed databases, object storage, Kubernetes, and other infrastructure-as-a-service products to developers and businesses.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/apis.yml)

## Timestamps

- **Modified:** 2026-05-19

## APIs

### Linode API V4

The Linode API v4 provides programmatic access to the full range of Akamai Connected Cloud (formerly Linode) products and services. It enables developers to create and manage compute instances, deploy Kubernetes clusters, configure NodeBalancers, manage DNS domains, provision Block Storage volumes, control Object Storage buckets, set up firewalls, and administer account settings.

- **Human URL:** [https://techdocs.akamai.com/linode-api/reference/api](https://techdocs.akamai.com/linode-api/reference/api)
- **Base URL:** `https://api.linode.com/v4`

#### Tags

- Cloud Computing
- Infrastructure
- REST API
- Virtual Machines

#### Properties

- [Documentation](https://techdocs.akamai.com/linode-api/reference/api)
- [OpenAPI](openapi/linode-api-v4-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/linode-api-v4.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/linode-api-v4.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Linode CLI

The Linode CLI is a command-line interface that wraps the Linode API v4, allowing developers and system administrators to manage Akamai Connected Cloud resources directly from the terminal. It supports all API operations including creating and managing compute instances, configuring networking, deploying Kubernetes clusters, and managing storage.

- **Human URL:** [https://techdocs.akamai.com/cloud-computing/docs/cli](https://techdocs.akamai.com/cloud-computing/docs/cli)
- **Base URL:** `https://api.example.com`

#### Tags

- Automation
- CLI
- Command Line
- DevOps

#### Properties

- [Documentation](https://techdocs.akamai.com/cloud-computing/docs/cli)
- [Postman Collection](collections/linode-api-v4.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/linode-api-v4.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Linode Python SDK

The Linode Python SDK (linode_api4) is the official Python client library for interacting with the Linode API v4. It provides a Pythonic interface for managing all Akamai Connected Cloud resources including compute instances, domains, NodeBalancers, volumes, Kubernetes clusters, and account settings. The SDK supports both synchronous operations and includes helper methods for common workflows like deploying instances from StackScripts, managing SSH keys, and configuring networking resources.

- **Human URL:** [https://linode-api4.readthedocs.io/en/latest/](https://linode-api4.readthedocs.io/en/latest/)
- **Base URL:** `https://api.example.com`

#### Tags

- Client Library
- Python
- SDK

#### Properties

- [Documentation](https://linode-api4.readthedocs.io/en/latest/)
- [Postman Collection](collections/linode-api-v4.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/linode-api-v4.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Linode Go SDK

The Linode Go SDK (linodego) is the official Go client library for the Linode API v4. It provides idiomatic Go interfaces for managing Akamai Connected Cloud infrastructure programmatically, including compute instances, Kubernetes clusters, networking configurations, storage volumes, and DNS domains. The library is used internally by the Linode Terraform Provider and Linode CLI, and supports context-based request cancellation, pagination helpers, and retry logic for robust API interactions.

- **Human URL:** [https://pkg.go.dev/github.com/linode/linodego](https://pkg.go.dev/github.com/linode/linodego)
- **Base URL:** `https://api.example.com`

#### Tags

- Client Library
- Go
- SDK

#### Properties

- [Documentation](https://pkg.go.dev/github.com/linode/linodego)
- [Postman Collection](collections/linode-api-v4.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/linode-api-v4.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Linode Terraform Provider

The Linode Terraform Provider enables infrastructure-as-code management of Akamai Connected Cloud resources using HashiCorp Terraform. It supports provisioning and managing compute instances, Kubernetes clusters, NodeBalancers, firewalls, DNS domains, Block Storage volumes, Object Storage buckets, VPCs, and other cloud resources through declarative configuration files.

- **Human URL:** [https://techdocs.akamai.com/terraform/docs/overview](https://techdocs.akamai.com/terraform/docs/overview)
- **Base URL:** `https://api.example.com`

#### Tags

- Automation
- DevOps
- Infrastructure as Code
- Terraform

#### Properties

- [Documentation](https://techdocs.akamai.com/terraform/docs/overview)
- [Postman Collection](collections/linode-api-v4.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/linode-api-v4.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/linode)
- [JSON-LD](json-ld/linode-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON Schema](json-schema/linode-instance-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Features](undefined)
