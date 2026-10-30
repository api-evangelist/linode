# Linode

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

Linode — operating as Akamai Cloud since Akamai's acquisition, with the Linode brand retained on the API, the CLI and the developer surface — is a cloud infrastructure provider offering virtual compute instances, GPU and accelerated plans, managed Kubernetes (LKE), S3-compatible Object Storage, Block Storage volumes, NodeBalancers, VPCs, Cloud Firewalls, managed MySQL/PostgreSQL/Valkey databases and DNS hosting. The Linode API v4 is a single cohesive REST surface at api.linode.com/v4 covering all of it: 358 paths and 539 operations in the first-party OpenAPI, documented at techdocs.akamai.com, with a generated CLI, first-party SDKs in Python, Go and TypeScript, a Terraform provider and an official read-only MCP server. Its price book is published as an unauthenticated API, so a stack can be costed with no account at all.

**Areas:** Cloud Computing · Infrastructure-as-a-Service · Virtual Machines · Kubernetes · Object Storage · Block Storage · DNS · Managed Database · Networking · GPU · Load Balancer · Developer Tools

## Linode on APIs.io

Everything profiled for Linode is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/linode/](https://apis.io/providers/linode/)** — or go straight to one of the APIs or properties below.

### APIs (127)

- [Linode CLI](https://apis.io/apis/linode/cli/) — The Linode CLI is a command-line interface that wraps the Linode API v4, allowing developers and system administrators to manage Akamai Connected Cloud…
- [Linode Python SDK](https://apis.io/apis/linode/python-sdk/) — The Linode Python SDK (linode_api4) is the official Python client library for interacting with the Linode API v4. It provides a Pythonic interface for…
- [Linode Go SDK](https://apis.io/apis/linode/go-sdk/) — The Linode Go SDK (linodego) is the official Go client library for the Linode API v4. It provides idiomatic Go interfaces for managing Akamai Connected…
- [Linode Terraform Provider](https://apis.io/apis/linode/terraform-provider/) — The Linode Terraform Provider enables infrastructure-as-code management of Akamai Connected Cloud resources using HashiCorp Terraform. It supports…
- [linode Account API](https://apis.io/apis/linode/linode-account-api/) — Manage your account settings, users, billing information, OAuth clients, service transfers, and payment methods.
- [linode Databases API](https://apis.io/apis/linode/linode-databases-api/) — Manage Managed Database instances including MySQL and PostgreSQL clusters, backups, credentials, and maintenance windows.
- [linode Domains API](https://apis.io/apis/linode/linode-domains-api/) — Manage DNS domains and their associated resource records including A, AAAA, CNAME, MX, TXT, SRV, CAA, and NS records.
- [linode Images API](https://apis.io/apis/linode/linode-images-api/) — Manage custom images for deploying Linode instances, including creating images from disks, uploading images, and managing image metadata.
- [linode Instances API](https://apis.io/apis/linode/linode-linode-instances-api/) — Create and manage Linode compute instances, including configuration profiles, disks, backups, networking, migration, resize, and rebuild operations.
- [linode Kubernetes Engine (LKE) API](https://apis.io/apis/linode/linode-linode-kubernetes-engine-lke-api/) — Deploy and manage Kubernetes clusters, node pools, and cluster configurations through the Linode Kubernetes Engine.
- [linode Longview API](https://apis.io/apis/linode/linode-longview-api/) — Manage Longview clients and subscriptions for system-level monitoring and metrics collection on Linode instances.
- [linode Managed API](https://apis.io/apis/linode/linode-managed-api/) — Manage Linode Managed services including monitored contacts, credentials, issues, service monitors, and SSH access settings.
- [linode Networking API](https://apis.io/apis/linode/linode-networking-api/) — Manage networking resources including IP addresses, IPv6 ranges and pools, firewalls, VLANs, and IP address sharing and assignment.
- [linode NodeBalancers API](https://apis.io/apis/linode/linode-nodebalancers-api/) — Create and manage NodeBalancer load balancers, their configurations, and backend nodes for distributing traffic across Linode instances.
- [linode Object Storage API](https://apis.io/apis/linode/linode-object-storage-api/) — Manage Object Storage buckets, access keys, clusters, and endpoints for S3-compatible object storage.
- [linode Placement Groups API](https://apis.io/apis/linode/linode-placement-groups-api/) — Create and manage placement groups for controlling the physical placement of Linode instances within a data center.
- [linode Profile API](https://apis.io/apis/linode/linode-profile-api/) — Manage your user profile settings, SSH keys, authorized applications, personal access tokens, and two-factor authentication.
- [linode Regions API](https://apis.io/apis/linode/linode-regions-api/) — List available data center regions and their capabilities for deploying Linode services.
- [linode StackScripts API](https://apis.io/apis/linode/linode-stackscripts-api/) — Create and manage StackScripts for automating the deployment and configuration of Linode instances.
- [linode Support API](https://apis.io/apis/linode/linode-support-api/) — Create and manage support tickets and view replies for getting help from the Linode support team.
- [linode Tags API](https://apis.io/apis/linode/linode-tags-api/) — The Tags API from linode — 2 operation(s) for tags.
- [linode Volumes API](https://apis.io/apis/linode/linode-volumes-api/) — Create and manage Block Storage volumes that can be attached to Linode instances for persistent data storage.
- [linode VPCs API](https://apis.io/apis/linode/linode-vpcs-api/) — Create and manage Virtual Private Clouds for isolated network environments and subnets for Linode instances.
- [Linode Access keys API](https://apis.io/apis/linode/linode-access-keys-api/) — Object Storage keys are used to authenticate access to your Object Storage buckets. Use these operations to create, view, update, and revoke these keys.
- [Linode Account agreements API](https://apis.io/apis/linode/linode-account-agreements-api/) — Use these operations to review and manage any agreements you need to acknowledge to use the API's services.
- [Linode Account availability API](https://apis.io/apis/linode/linode-account-availability-api/) — Use these operations to review the services available for use with your account.
- [Linode Account logins API](https://apis.io/apis/linode/linode-account-logins-api/) — Use these operations to review successful login data.
- [Linode Account settings API](https://apis.io/apis/linode/linode-account-settings-api/) — Account settings applies to various services available on your account, including Backups, Linode Interfaces, a Longview subscription, Maintenance Policy,…
- [Linode Account transfer API](https://apis.io/apis/linode/linode-account-transfer-api/) — Used to manage transfer objects that show your network utilization.
- [Linode Alerts API](https://apis.io/apis/linode/linode-alerts-api/) — Akamai Cloud Pulse lets you configure alerts to monitor key metrics and events in real time and automatically trigger notifications or actions when…
- [Linode Attachments API](https://apis.io/apis/linode/linode-attachments-api/) — Mange any attachments you may need to include with your support tickets, such as log entry files and screenshot images.
- [Linode Buckets API](https://apis.io/apis/linode/linode-buckets-api/) — Buckets are the primary containers within Object Storage. Each bucket stores your files (objects) and lets you access or share those files. Use these…
- [Linode Child accounts API](https://apis.io/apis/linode/linode-child-accounts-api/) — Child accounts let you, as an Akamai partner (a parent account holder), switch between and manage your end customers' accounts (child accounts). Talk to…
- [Linode Configuration profile interfaces API](https://apis.io/apis/linode/linode-configuration-profile-interfaces-api/) — Use these operations to upgrade and manage a legacy configuration profile on your Linode to include networking interfaces.
- [Linode Configuration profiles API](https://apis.io/apis/linode/linode-configuration-profiles-api/) — A configuration profile establishes the disk layout, kernel installation, and other specifics for a Linode. This is the legacy method used to define a…
- [Linode Configurations API](https://apis.io/apis/linode/linode-configurations-api/) — The Configurations API from Linode — 3 operation(s) for configurations.
- [Linode Control Plane ACL API](https://apis.io/apis/linode/linode-control-plane-acl-api/) — View and manage access control lists (ACLs) for the control planes on your LKE clusters. Control Plane ACLs allow you to restrict access to your cluster's…
- [Linode Delegation for parent and child accounts API](https://apis.io/apis/linode/linode-delegation-for-parent-and-child-accounts-api/) — Use these operations to manage delegations for [parent and child…
- [Linode Devices API](https://apis.io/apis/linode/linode-devices-api/) — The Devices API from Linode — 2 operation(s) for devices.
- [Linode Domain records API](https://apis.io/apis/linode/linode-domain-records-api/) — Use these operations to create and manage domain records on your account.
- [Linode Domain zone files API](https://apis.io/apis/linode/linode-domain-zone-files-api/) — These operations involve viewing specifics for a domain zone file.
- [Linode Endpoints API](https://apis.io/apis/linode/linode-endpoints-api/) — An endpoint is the S3-compatible URL to an Object Storage bucket. Use these operations to review details about your endpoints.
- [Linode Entity transfers API](https://apis.io/apis/linode/linode-entity-transfers-api/) — These legacy operations are available to review and manage the transfer of one entity to another. These operations have been deprecated. Use the Service…
- [Linode Events API](https://apis.io/apis/linode/linode-events-api/) — An event represents an action you've taken on your account, over the last 90 days. Use these operations to review your current events.
- [Linode Firewall settings API](https://apis.io/apis/linode/linode-firewall-settings-api/) — The Firewall settings API from Linode — 1 operation(s) for firewall settings.
- [Linode Firewalls API](https://apis.io/apis/linode/linode-firewalls-api/) — The Firewalls API from Linode — 6 operation(s) for firewalls.
- [Linode General API](https://apis.io/apis/linode/linode-general-api/) — Object Storage is Akamai cloud computing's S3-compatible data storage service. Use these operations to review and manage your Object Storage service.
- [Linode Grants API](https://apis.io/apis/linode/linode-grants-api/) — View the grants (permissions) available to your user account.
- [Linode Identity Management API](https://apis.io/apis/linode/linode-identity-management-api/) — Use these operations to manage access to entities and roles on your account.
- [Linode IDP configuration API](https://apis.io/apis/linode/linode-idp-configuration-api/) — Use the Identity Management IDP Configuration endpoints to configure SAML-based Single Sign-On (SSO) for your account. You can create and manage an external…
- [Linode Image sharing API](https://apis.io/apis/linode/linode-image-sharing-api/) — Use these operations to create and mange groups of users that can access your stored images.
- [Linode Invoices API](https://apis.io/apis/linode/linode-invoices-api/) — Review invoice and billing data for services on your account.
- [Linode IP addresses API](https://apis.io/apis/linode/linode-ip-addresses-api/) — Use the IP addresses endpoints to view Virtual Private Cloud (VPC): - IP addresses - default address ranges - forbidden CIDR blocks for your environment
- [Linode IPv4 addresses API](https://apis.io/apis/linode/linode-ipv4-addresses-api/) — The IPv4 addresses API from Linode — 2 operation(s) for ipv4 addresses.
- [Linode IPv6 pools API](https://apis.io/apis/linode/linode-ipv6-pools-api/) — The IPv6 pools API from Linode — 1 operation(s) for ipv6 pools.
- [Linode IPv6 ranges API](https://apis.io/apis/linode/linode-ipv6-ranges-api/) — The IPv6 ranges API from Linode — 2 operation(s) for ipv6 ranges.
- [Linode Kubeconfigs API](https://apis.io/apis/linode/linode-kubeconfigs-api/) — View or regenerate the kubeconfig files for your LKE clusters, which authenticate and configure access to your Kubernetes clusters.
- [Linode Legacy clusters API](https://apis.io/apis/linode/linode-legacy-clusters-api/) — Clusters refer to the legacy methodology Object Storage used, before moving Object Storage to our actual data centers (regions). These operations have been…
- [Linode Linode disk backups API](https://apis.io/apis/linode/linode-linode-disk-backups-api/) — The Backups service lets you enable automatic backups of the disks on your Linodes. Use these operations to manage your backups.
- [Linode Linode disks API](https://apis.io/apis/linode/linode-linode-disks-api/) — Use these operations to manage the individual disks on your Linode.
- [Linode Linode firewalls API](https://apis.io/apis/linode/linode-linode-firewalls-api/) — Use these operations to manage the firewalls applied to your Linodes.
- [Linode Linode interfaces API](https://apis.io/apis/linode/linode-linode-interfaces-api/) — A Linode interface lets you set up networking on your Linode. A Linode interface links to the Linode, rather than to a legacy configuration profile. Use…
- [Linode Linode IP addresses API](https://apis.io/apis/linode/linode-linode-ip-addresses-api/) — Use these operations to view and manage the IP addresses assigned to your Linodes.
- [Linode Linode kernels API](https://apis.io/apis/linode/linode-linode-kernels-api/) — Use these operations to review information for the Linux kernels on your Linodes.
- [Linode Linode NodeBalancers API](https://apis.io/apis/linode/linode-linode-nodebalancers-api/) — A NodeBalancer is a managed load balancer that intelligently distributes incoming requests to multiple backend Linodes, so that there's no single point of…
- [Linode Linode statistics API](https://apis.io/apis/linode/linode-linode-statistics-api/) — Use these operations to review various statistics for your Linodes.
- [Linode Linode types API](https://apis.io/apis/linode/linode-linode-types-api/) — Use these operations to get information about Linode plan types, including pricing information, hardware resources, and network transfer allotment.
- [Linode Linode volumes API](https://apis.io/apis/linode/linode-linode-volumes-api/) — The Block Storage service lets you add storage drives, called volumes to your Linodes. This lets you store more data without resizing your Linode to a…
- [Linode LKE API endpoints API](https://apis.io/apis/linode/linode-lke-api-endpoints-api/) — View the API endpoints for your LKE clusters.
- [Linode LKE cluster dashboard API](https://apis.io/apis/linode/linode-lke-cluster-dashboard-api/) — View the Kubernetes Dashboard URLs for your LKE clusters, which provides a web-based user interface for managing and monitoring each Kubernetes cluster.
- [Linode LKE clusters API](https://apis.io/apis/linode/linode-lke-clusters-api/) — Create and manage Kubernetes clusters on LKE (Linode Kubernetes Engine).
- [Linode LKE node pools API](https://apis.io/apis/linode/linode-lke-node-pools-api/) — Create, manage, and configure node pools within your LKE clusters. Node pools allow you to group nodes with similar configurations and manage them collectively.
- [Linode LKE nodes API](https://apis.io/apis/linode/linode-lke-nodes-api/) — View, recycle, and delete nodes within your LKE clusters. Nodes are the worker machines in your Kubernetes cluster that run your containerized applications.
- [Linode LKE service tokens API](https://apis.io/apis/linode/linode-lke-service-tokens-api/) — Regenerate service account tokens for your LKE clusters, which are used by the cluster's control plane components and Linode CSI drivers to authenticate…
- [Linode LKE types API](https://apis.io/apis/linode/linode-lke-types-api/) — View the LKE tiers (types) available for your Kubernetes clusters. The cluster tier determines the control plane configuration and features available for…
- [Linode LKE versions API](https://apis.io/apis/linode/linode-lke-versions-api/) — View the Kubernetes versions available for deployment on your LKE clusters.
- [Linode Logs API](https://apis.io/apis/linode/linode-logs-api/) — Akamai Cloud Pulse lets you capture log data across multiple Akamai Cloud services and deliver it to the destination of your choice. These logs can help you…
- [Linode Longview clients API](https://apis.io/apis/linode/linode-longview-clients-api/) — Create an manage Longview Clients to monitor the performance and health of your Linode instances and other servers.
- [Linode Longview plans API](https://apis.io/apis/linode/linode-longview-plans-api/) — Get details on your current Longview plan subscription and, if needed, update your plan.
- [Linode Longview subscriptions API](https://apis.io/apis/linode/linode-longview-subscriptions-api/) — Get publicly-accessible information about the Longview plans available on Akamai Cloud, including the number of supported clients.
- [Linode Longview types API](https://apis.io/apis/linode/linode-longview-types-api/) — Get publicly-accessible information about the Longview plans available on Akamai Cloud, including network transfer and region-specific pricing.
- [Linode Maintenance policies API](https://apis.io/apis/linode/linode-maintenance-policies-api/) — Use these operations to view maintenance policies that are available for your Linodes.
- [Linode Maintenances API](https://apis.io/apis/linode/linode-maintenances-api/) — Review details on scheduled maintenance for your Akamai Cloud Computing services.
- [Linode Manage Beta programs API](https://apis.io/apis/linode/linode-manage-beta-programs-api/) — Use these operations to view information about available beta programs and sign up to participate in them.
- [Linode Managed contacts API](https://apis.io/apis/linode/linode-managed-contacts-api/) — Create and manage contacts associated with Linode Managed, who can be notified about issues with your managed Linodes.
- [Linode Managed credentials API](https://apis.io/apis/linode/linode-managed-credentials-api/) — Create and manage credentials used by Linode Managed to access your Linodes for support and maintenance.
- [Linode Managed issues API](https://apis.io/apis/linode/linode-managed-issues-api/) — View details about issues detected on your managed Linodes and their resolution status.
- [Linode Managed Linode settings API](https://apis.io/apis/linode/linode-managed-linode-settings-api/) — View and update settings related to Linode Managed for each of your Linodes.
- [Linode Managed service monitors API](https://apis.io/apis/linode/linode-managed-service-monitors-api/) — Create and configure the service monitors that are used to check the health of your managed Linodes.
- [Linode Managed SSH keys API](https://apis.io/apis/linode/linode-managed-ssh-keys-api/) — View the unique SSH public key assigned to your Linode Managed account.
- [Linode Managed statistics API](https://apis.io/apis/linode/linode-managed-statistics-api/) — View key metrics for your managed Linodes, including CPU usage, disk I/O, and network transfer.
- [Linode Metrics API](https://apis.io/apis/linode/linode-metrics-api/) — Akamai Cloud Pulse automatically collects and stores performance metrics for your cloud services. You can view them through dashboards and inspect them at…
- [Linode My SQL API](https://apis.io/apis/linode/linode-mysql-api/) — Managed Databases is Akamai's fully-managed, high-performance database service. Use these operations to create and manage clusters for MySQL engine databases.
- [Linode Network transfer prices API](https://apis.io/apis/linode/linode-network-transfer-prices-api/) — Review network transfer pricing information.
- [Linode NodeBalancer types API](https://apis.io/apis/linode/linode-nodebalancer-types-api/) — The NodeBalancer types API from Linode — 1 operation(s) for nodebalancer types.
- [Linode Nodes API](https://apis.io/apis/linode/linode-nodes-api/) — The Nodes API from Linode — 2 operation(s) for nodes.
- [Linode Notifications API](https://apis.io/apis/linode/linode-notifications-api/) — Review notifications that represent important, often time-sensitive details about your account.
- [Linode OAuth apps API](https://apis.io/apis/linode/linode-oauth-apps-api/) — View authorized apps that have been granted access to your account. You can also revoke access for any authorized app.
- [Linode OAuth clients API](https://apis.io/apis/linode/linode-oauth-clients-api/) — Use an OAuth client to allow users (using their Akamai Cloud Computing account) to log in to your own application, and optionally grant your application…
- [Linode OAuth preferences API](https://apis.io/apis/linode/linode-oauth-preferences-api/) — View and update user preferences tied to OAuth clients.
- [Linode Partner referrals API](https://apis.io/apis/linode/linode-partner-referrals-api/) — The Marketplace offers the Partner referrals program. This is a new space for Akamai qualified partners to offer their products to Cloud Manager customers.
- [Linode Payment methods API](https://apis.io/apis/linode/linode-payment-methods-api/) — Use these operations to review and manage the payment method you've set up to pay your invoices.
- [Linode Payments API](https://apis.io/apis/linode/linode-payments-api/) — Use these operations to view current payment due information and make a payment.
- [Linode Personal access tokens API](https://apis.io/apis/linode/linode-personal-access-tokens-api/) — Manage personal access tokens for your user account. Personal access tokens can be used for authentication with the Linode API.
- [Linode Phone number API](https://apis.io/apis/linode/linode-phone-number-api/) — Operations to verify and delete the phone number associated with your user account, which is used to send SMS messages as a form of two-factor…
- [Linode Postgre SQL API](https://apis.io/apis/linode/linode-postgresql-api/) — Managed Databases is Akamai's fully-managed, high-performance database service. Use these operations to create and manage clusters for PostgreSQL engine…
- [Linode Prefix Lists API](https://apis.io/apis/linode/linode-prefix-lists-api/) — The Prefix Lists API from Linode — 3 operation(s) for prefix lists.
- [Linode Profile logins API](https://apis.io/apis/linode/linode-profile-logins-api/) — View a history of successful logins to your Linode account.
- [Linode Promo credits API](https://apis.io/apis/linode/linode-promo-credits-api/) — Use these operations to manage any promotional codes you've been granted for special offers.
- [Linode Quotas API](https://apis.io/apis/linode/linode-quotas-api/) — Quotas are limits related to your resource usage in Object Storage. Use these operations to review and manage your Object Storage quotas.
- [Linode Replies API](https://apis.io/apis/linode/linode-replies-api/) — Use these operations to create and view replies to correspondence for your support tickets.
- [Linode Reserved IPs API](https://apis.io/apis/linode/linode-reserved-ips-api/) — The Reserved IPs API from Linode — 3 operation(s) for reserved ips.
- [Linode Resource locks API](https://apis.io/apis/linode/linode-resource-locks-api/) — Add and manage locks on your Akamai Cloud resources to prevent you from inadvertently deleting them.
- [Linode Review Beta programs API](https://apis.io/apis/linode/linode-review-beta-programs-api/) — Use these operations to view information about available beta programs. You can sign up to participate in one of these programs using the [Enroll in a Beta…
- [Linode Security questions API](https://apis.io/apis/linode/linode-security-questions-api/) — View and configure security questions for your user account. Security questions can be used to help verify your identity when contacting Akamai Support.
- [Linode Service transfers API](https://apis.io/apis/linode/linode-service-transfers-api/) — Use these operations to manage transfer requests for specific Akamai Cloud Computing services. For example, you could request a service transfer to move a…
- [Linode SSH keys API](https://apis.io/apis/linode/linode-ssh-keys-api/) — Manage SSH keys for your user account. When creating a Linode, you can choose to have one or more SSH keys automatically added to the new Linode for secure…
- [Linode Support tickets API](https://apis.io/apis/linode/linode-support-tickets-api/) — Use these operations to open, view, and close support tickets, when you need assistance from Akamai.
- [Linode Templates API](https://apis.io/apis/linode/linode-templates-api/) — The Templates API from Linode — 2 operation(s) for templates.
- [Linode Trusted devices API](https://apis.io/apis/linode/linode-trusted-devices-api/) — View details about trusted devices associated with your user account. If needed, you can revoke a trusted device so any future login attempts from that…
- [Linode Two-factor authentication (2FA) API](https://apis.io/apis/linode/linode-two-factor-authentication-2fa-api/) — The Two-factor authentication (2FA) API from Linode — 4 operation(s) for two-factor authentication (2fa).
- [Linode Users API](https://apis.io/apis/linode/linode-users-api/) — Users are individuals on your account that you set up to perform specific tasks. Use these operations to view and manage users, including giving them…
- [Linode Valkey API](https://apis.io/apis/linode/linode-valkey-api/) — Managed Databases is Akamai's fully-managed, high-performance database service. Use these operations to create and manage clusters for Valkey engine databases.
- [Linode VLANs API](https://apis.io/apis/linode/linode-vlans-api/) — The VLANs API from Linode — 2 operation(s) for vlans.
- [Linode Volume types API](https://apis.io/apis/linode/linode-volume-types-api/) — Use these operations to review the available Block Storage volume types, including pricing.
- [Linode VPC subnets API](https://apis.io/apis/linode/linode-vpc-subnets-api/) — Use the VPC subnet endpoints to view, create, and manage Virtual Private Cloud (VPC) subnet resources.
- [Linode Rulesets API](https://apis.io/apis/linode/linode-rulesets-api/) — The Rulesets API from Linode — 2 operation(s) for rulesets.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [Akamai Cloud MCP Server](https://apis.io/servers/linode/akamai-cloud-mcp-server/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Linode Agentic Access](https://apis.io/agentic-access/linode/linode-agentic-access/)

#### JSON Schema (109)

The data models the API reads and writes.

- [Account](https://apis.io/schemas/linode/linode-account/)
- [Backup](https://apis.io/schemas/linode/linode-backup/)
- [BackupResponse](https://apis.io/schemas/linode/linode-backupresponse/)
- [Database](https://apis.io/schemas/linode/linode-database/)
- [DatabaseRequest](https://apis.io/schemas/linode/linode-databaserequest/)
- [Domain](https://apis.io/schemas/linode/linode-domain/)
- [DomainRecord](https://apis.io/schemas/linode/linode-domainrecord/)
- [DomainRecordRequest](https://apis.io/schemas/linode/linode-domainrecordrequest/)
- [DomainRequest](https://apis.io/schemas/linode/linode-domainrequest/)
- [Event](https://apis.io/schemas/linode/linode-event/)
- [Firewall](https://apis.io/schemas/linode/linode-firewall/)
- [FirewallRequest](https://apis.io/schemas/linode/linode-firewallrequest/)
- [FirewallRule](https://apis.io/schemas/linode/linode-firewallrule/)
- [FirewallUpdateRequest](https://apis.io/schemas/linode/linode-firewallupdaterequest/)
- [Image](https://apis.io/schemas/linode/linode-image/)
- [ImageRequest](https://apis.io/schemas/linode/linode-imagerequest/)
- [ImageUpdateRequest](https://apis.io/schemas/linode/linode-imageupdaterequest/)
- [Linode Instance](https://apis.io/schemas/linode/linode-instance/)
- [Invoice](https://apis.io/schemas/linode/linode-invoice/)
- [IPAddress](https://apis.io/schemas/linode/linode-ipaddress/)
- [IPv6Address](https://apis.io/schemas/linode/linode-ipv6address/)
- [IPv6Range](https://apis.io/schemas/linode/linode-ipv6range/)
- [KubernetesVersion](https://apis.io/schemas/linode/linode-kubernetesversion/)
- [Linode](https://apis.io/schemas/linode/linode-linode/)
- [LinodeIPAddresses](https://apis.io/schemas/linode/linode-linodeipaddresses/)
- …and 84 more published on APIs.io

#### JSON Structure (1)

Data models expressed in JSON Structure.

- [Linode Structure](https://apis.io/json-structure/linode/linode-structure/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Linode Context](https://apis.io/jsonld/linode/linode-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Linode Domain Vocabulary](https://apis.io/vocabularies/linode/linode-vocabulary/)

#### Collections (20)

Postman and Open Collection request collections.

- [Linode API v4 Account API](https://apis.io/collections/linode/open-linode-account-api/)
- [Linode API v4](https://apis.io/collections/linode/open-linode-api-v4/)
- [Linode API v4 Account Databases API](https://apis.io/collections/linode/open-linode-databases-api/)
- [Linode API v4 Account Domains API](https://apis.io/collections/linode/open-linode-domains-api/)
- [Linode API v4 Account Images API](https://apis.io/collections/linode/open-linode-images-api/)
- [Linode API v4 Account Linode Instances API](https://apis.io/collections/linode/open-linode-linode-instances-api/)
- [Linode API v4 Account Linode Kubernetes Engine (LKE) API](https://apis.io/collections/linode/open-linode-linode-kubernetes-engine-lke-api/)
- [Linode API v4 Account Longview API](https://apis.io/collections/linode/open-linode-longview-api/)
- [Linode API v4 Account Managed API](https://apis.io/collections/linode/open-linode-managed-api/)
- [Linode API v4 Account Networking API](https://apis.io/collections/linode/open-linode-networking-api/)
- [Linode API v4 Account NodeBalancers API](https://apis.io/collections/linode/open-linode-nodebalancers-api/)
- [Linode API v4 Account Object Storage API](https://apis.io/collections/linode/open-linode-object-storage-api/)
- [Linode API v4 Account Placement Groups API](https://apis.io/collections/linode/open-linode-placement-groups-api/)
- [Linode API v4 Account Profile API](https://apis.io/collections/linode/open-linode-profile-api/)
- [Linode API v4 Account Regions API](https://apis.io/collections/linode/open-linode-regions-api/)
- [Linode API v4 Account StackScripts API](https://apis.io/collections/linode/open-linode-stackscripts-api/)
- [Linode API v4 Account Support API](https://apis.io/collections/linode/open-linode-support-api/)
- [Linode API v4 Account Tags API](https://apis.io/collections/linode/open-linode-tags-api/)
- [Linode API v4 Account Volumes API](https://apis.io/collections/linode/open-linode-volumes-api/)
- [Linode API v4 Account VPCs API](https://apis.io/collections/linode/open-linode-vpcs-api/)

#### Overlays (19)

OpenAPI overlays, including conversational phrasing for each operation.

- [Linode Account Api Overlay](https://apis.io/overlays/linode/linode-account-api-overlay/)
- [Linode Databases Api Overlay](https://apis.io/overlays/linode/linode-databases-api-overlay/)
- [Linode Domains Api Overlay](https://apis.io/overlays/linode/linode-domains-api-overlay/)
- [Linode Images Api Overlay](https://apis.io/overlays/linode/linode-images-api-overlay/)
- [Linode Linode Instances Api Overlay](https://apis.io/overlays/linode/linode-linode-instances-api-overlay/)
- [Linode Linode Kubernetes Engine Lke Api Overlay](https://apis.io/overlays/linode/linode-linode-kubernetes-engine-lke-api-overlay/)
- [Linode Longview Api Overlay](https://apis.io/overlays/linode/linode-longview-api-overlay/)
- [Linode Managed Api Overlay](https://apis.io/overlays/linode/linode-managed-api-overlay/)
- [Linode Networking Api Overlay](https://apis.io/overlays/linode/linode-networking-api-overlay/)
- [Linode Nodebalancers Api Overlay](https://apis.io/overlays/linode/linode-nodebalancers-api-overlay/)
- [Linode Object Storage Api Overlay](https://apis.io/overlays/linode/linode-object-storage-api-overlay/)
- [Linode Placement Groups Api Overlay](https://apis.io/overlays/linode/linode-placement-groups-api-overlay/)
- [Linode Profile Api Overlay](https://apis.io/overlays/linode/linode-profile-api-overlay/)
- [Linode Regions Api Overlay](https://apis.io/overlays/linode/linode-regions-api-overlay/)
- [Linode Stackscripts Api Overlay](https://apis.io/overlays/linode/linode-stackscripts-api-overlay/)
- [Linode Support Api Overlay](https://apis.io/overlays/linode/linode-support-api-overlay/)
- [Linode Tags Api Overlay](https://apis.io/overlays/linode/linode-tags-api-overlay/)
- [Linode Volumes Api Overlay](https://apis.io/overlays/linode/linode-volumes-api-overlay/)
- [Linode Vpcs Api Overlay](https://apis.io/overlays/linode/linode-vpcs-api-overlay/)

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [Linode — jsonschema rules](https://apis.io/rules/linode/linode-jsonschema-spectral-rules/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Linode Authentication](https://apis.io/security/linode/linode-authentication/)
- [Linode Domain Security](https://apis.io/security/linode/linode-domain-security/)
- [Linode Vulnerability Disclosure](https://apis.io/security/linode/linode-vulnerability-disclosure/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Linode Scopes](https://apis.io/scopes/linode/linode-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Linode Plans Pricing](https://apis.io/plans/linode/linode-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Linode Rate Limits](https://apis.io/rate-limits/linode/linode-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Linode Finops](https://apis.io/finops/linode/linode-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.linode.com/)
- [Documentation](https://techdocs.akamai.com/linode-api/)
- [Getting started](https://techdocs.akamai.com/linode-api/reference/get-started)
- [API reference](https://techdocs.akamai.com/linode-api/reference/api)
- [Pricing](https://api.linode.com/v4/linode/types)
- [Sign up](https://login.linode.com/signup)
- [GitHub](https://github.com/linode)
- [Status](https://status.linode.com/)

## API Evangelist rating

**Kin Score 55.7** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 71.7 |
| Contract quality | 58.2 |
| Contract governance | 28.0 |
| Operational transparency | 84.2 |
| Developer ergonomics | 28.0 |
| Access clarity | 55.3 |

**Agent readiness 42.1** — agent-ready (gated down from agent-native)

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | documented (partial credit) |
| Auth Clarity | negotiable (partial credit) |
| Idempotency | — |
| Error Semantics | documented (partial credit) |
| OpenAPI Examples | verified |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | yes |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | yes |
| Delegated Identity | documented (partial credit) |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | — |

**Regulatory alignment 32.4** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/linode/](https://apis.io/providers/linode/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Linode: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/linode/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
