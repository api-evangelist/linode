# Linode (linode)
Linode, now part of Akamai Connected Cloud, is a cloud computing platform that provides virtual machines, Kubernetes, storage, networking, and other infrastructure services. Their developer platform offers a comprehensive REST API, CLI tools, SDKs, and a Terraform provider for programmatic management of cloud resources.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/apis.yml)

## Scope

- **Type:** Contract
- **Position:** Consuming
- **Access:** 3rd-Party

## Tags:

 - Cloud Computing, Infrastructure, Virtual Machines, DevOps, Infrastructure As Code

## Timestamps

- **Created:** 2026-03-20
- **Modified:** 2026-03-20

## APIs

### Linode API v4
The Linode API v4 provides programmatic access to the full range of Akamai Connected Cloud (formerly Linode) products and services. It enables developers to create and manage compute instances, deploy Kubernetes clusters, configure NodeBalancers, manage DNS domains, provision Block Storage volumes, control Object Storage buckets, set up firewalls, and administer account settings. The RESTful API uses OAuth for authentication and returns JSON responses, with support for filtering and sorting across all resource endpoints.

**Human URL:** [https://techdocs.akamai.com/linode-api/reference/api](https://techdocs.akamai.com/linode-api/reference/api)


#### Tags:

 - Cloud Computing, Infrastructure, Virtual Machines, REST API

#### Properties

- [Documentation](https://techdocs.akamai.com/linode-api/reference/api)
- [OpenAPI](openapi/linode-api-v4-openapi.yml)

### Linode CLI
The Linode CLI is a command-line interface that wraps the Linode API v4, allowing developers and system administrators to manage Akamai Connected Cloud resources directly from the terminal. It supports all API operations including creating and managing compute instances, configuring networking, deploying Kubernetes clusters, and managing storage. The CLI is installed via pip and auto-generates its command structure from the Linode API OpenAPI specification, ensuring it stays current with the latest API features.

**Human URL:** [https://techdocs.akamai.com/cloud-computing/docs/cli](https://techdocs.akamai.com/cloud-computing/docs/cli)


#### Tags:

 - Command Line, CLI, DevOps, Automation

#### Properties

- [Documentation](https://techdocs.akamai.com/cloud-computing/docs/cli)

### Linode Python SDK
The Linode Python SDK (linode_api4) is the official Python client library for interacting with the Linode API v4. It provides a Pythonic interface for managing all Akamai Connected Cloud resources including compute instances, domains, NodeBalancers, volumes, Kubernetes clusters, and account settings. The SDK supports both synchronous operations and includes helper methods for common workflows like deploying instances from StackScripts, managing SSH keys, and configuring networking resources.

**Human URL:** [https://linode-api4.readthedocs.io/en/latest/](https://linode-api4.readthedocs.io/en/latest/)


#### Tags:

 - Python, SDK, Client Library

#### Properties

- [Documentation](https://linode-api4.readthedocs.io/en/latest/)

### Linode Go SDK
The Linode Go SDK (linodego) is the official Go client library for the Linode API v4. It provides idiomatic Go interfaces for managing Akamai Connected Cloud infrastructure programmatically, including compute instances, Kubernetes clusters, networking configurations, storage volumes, and DNS domains. The library is used internally by the Linode Terraform Provider and Linode CLI, and supports context-based request cancellation, pagination helpers, and retry logic for robust API interactions.

**Human URL:** [https://pkg.go.dev/github.com/linode/linodego](https://pkg.go.dev/github.com/linode/linodego)


#### Tags:

 - Go, SDK, Client Library

#### Properties

- [Documentation](https://pkg.go.dev/github.com/linode/linodego)

### Linode Terraform Provider
The Linode Terraform Provider enables infrastructure-as-code management of Akamai Connected Cloud resources using HashiCorp Terraform. It supports provisioning and managing compute instances, Kubernetes clusters, NodeBalancers, firewalls, DNS domains, Block Storage volumes, Object Storage buckets, VPCs, and other cloud resources through declarative configuration files. The provider is currently at version 3.0, which supports the latest Akamai Cloud platform features and integrates with Terraform workflows for planning, applying, and destroying infrastructure.

**Human URL:** [https://techdocs.akamai.com/terraform/docs/overview](https://techdocs.akamai.com/terraform/docs/overview)


#### Tags:

 - Terraform, Infrastructure As Code, DevOps, Automation

#### Properties

- [Documentation](https://techdocs.akamai.com/terraform/docs/overview)

## Common Properties

- [Portal](https://techdocs.akamai.com/cloud-computing/docs)
- [Documentation](https://techdocs.akamai.com/linode-api/reference/api)
- [Website](https://www.linode.com/)
- [PrivacyPolicy](https://www.linode.com/legal-privacy/)
- [TermsOfService](https://www.linode.com/legal-tos/)
- [Support](https://www.linode.com/support/)
- [Blog](https://www.linode.com/blog/)
- [Login](https://login.linode.com/login)

## Maintainers

**FN:** API Evangelist

**Email:** info@apievangelist.com
