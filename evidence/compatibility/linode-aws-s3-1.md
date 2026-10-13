<!-- fetched 2026-10-13 from https://techdocs.akamai.com/cloud-computing/docs/object-storage by sweep-shape-compat.py; text extracted from the provider's own page -->

Overview For AI agents: visit https://techdocs.akamai.com/cloud-computing/llms.txt for an index of all pages formatted in Markdown and endpoints in OpenAPI. Append .md to any documentation page URL to get its markdown version.
 Jump to Content 
 Guide Release notes API CLI Cloud Manager Tutorials Support Community 
 Guide
 Guide Release notes API CLI Cloud Manager Tutorials Support Community 
 Overview 
 Platform
 Akamai Cloud 
 Get started Choose a data center 
 Network transfer usage and costs 
 Help & support 
 Send email on Akamai Cloud 
 Subscribe to status updates 
 Grant a developer access to your services 
 Automate cloud resource deployment 
 Resell services 
 Distributed compute regions (limited availability) Supported services 
 Plans 
 IP Sharing and failover in distributed compute regions 
 Create a Linode in a distributed compute region 
 New data centers 2026 
 NVIDIA RTX PRO 6000 Blackwell GPU Onboarding (limited availability) 
 Profile Security controls for user accounts 
 Manage 2FA on a user account 
 Enable third-party authentication on your user account 
 Manage SSH keys 
 Manage personal access tokens 
 Reset your user password 
 Profile FAQ 
 Administration Manage users on your account 
 Change your email address on your account 
 Transfer services to a different account 
 Parent and child accounts for Akamai partners 
 Select network interfaces for new Linodes 
 Select default Cloud Firewalls for new Linodes 
 Cancel your account 
 Quotas 
 Billing Access billing information 
 View invoices and payment history 
 Update billing contact information 
 Make a payment 
 Manage payment methods 
 Stop further billing 
 Tax information 
 Referral program 
 Add a promo code 
 Billing FAQ 
 Identity and Access
 Identity and Access in Akamai Cloud Migration from grants to Identity and Access Grants vs RBAC model comparison: Linodes example 
 Manage user access 
 Available roles 
 Single sign-on for Akamai Cloud Configure single sign-on Enable single sign-on 
 Enforce single sign-on 
 Test the IDP configuration 
 Add SSO User Exceptions 
 Add SSO-required users 
 Configure IDP settings Create an identity provider (IDP) configuration 
 Manage certificates 
 Delete an identity provider (IDP) configuration 
 Two-factor authentication (2FA) for Akamai Cloud Enforce two-factor authentication (2FA) for the account 
 Make two-factor authentication (2FA) optional 
 Delegation for parent and child accounts Partners 
 End customers 
 Migrated partners 
 Migrated end customers 
 Identity and Access audit logs 
 Compute
 Linodes Get started with Linodes 
 Create a Linode 
 Disk encryption 
 Set up and secure a Linode 
 Plans Generational compute plans 
 Choose a compute plan 
 Choose between shared and dedicated CPUs 
 Dedicated CPU Linodes 
 Shared CPU Linodes 
 High Memory Linodes 
 Premium Linodes 
 Accelerated Linodes 
 GPU Linodes 
 GPU selection guidance 
 vNUMA topology 
 Install the NVIDIA CUDA toolkit on GPU Linodes 
 Resize a Linode 
 Known limitations you may encounter with NVIDIA RTX PRO 6000 Blackwell Server Edition GPU Linodes 
 Choose a Linux distribution Default distro packages 
 Package mirrors 
 Manage disks and storage on a Linode Copy a disk over SSH 
 Copy a disk to a different account 
 Reset the root password on a Linode 
 Clone a Linode 
 Access your system console using Lish 
 Access your desktop environment using Glish 
 Networking Automatically configure networking (Network Helper) 
 DNS resolvers 
 Manage IP addresses on a Linode 
 IPv6 on Linodes 
 Configure rDNS (reverse DNS) on a Linode 
 Enable IP sharing (elastic IPs) in Atlanta through FRR 
 Configure failover on a Linode 
 Configure IP failover over BGP using FRR (advanced) 
 Use keepalived health checks with BGP-based failover 
 Configure multi-queue NICs on Linodes 
 Manage configuration profiles on a Linode Manage the kernel on a Linode 
 Networking interfaces Manage Linode interfaces 
 Manage configuration profile interfaces 
 Upgrade configuration profile interfaces to Linode interfaces 
 Manual network configuration on a Linode Network configuration using NetworkManager 
 Network configuration using Netplan 
 Network configuration using ifupdown 
 Network configuration using systemd-networkd 
 Work with placement groups 
 Monitor and maintain Linodes Configure email alerts for resource usage on Linodes 
 Linodes audit logs 
 Update system packages 
 Recovery and troubleshooting Recover from unexpected shutdowns with Lassie 
 Rescue and rebuild 
 Troubleshooting general issues on Linodes 
 Troubleshooting basic connection issues on Linodes 
 Troubleshooting SSH on Linodes 
 Troubleshooting memory issues on Linodes 
 Troubleshooting firewall issues on Linodes 
 Troubleshooting web servers, databases, and other services 
 Migrations within Akamai Cloud Migrate to a new data center 
 Maintenance events and policies 
 Linodes FAQs 
 Linode Managed Get started with Linode Managed 
 Configure credentials for Linode Managed 
 Configure SSH access for Linode Managed 
 Configure firewall rules to allow access for Linode Managed 
 Create and edit service monitors for Linode Managed 
 Manage contacts for Linode Managed 
 Cancel Linode Managed 
 Linode Kubernetes Engine LKE Enterprise Known issues you may encounter with LKE Enterprise 
 Upgrade an LKE Enterprise cluster to a newer Kubernetes version 
 Getting started with LKE 
 Create a cluster 
 Manage Kubernetes clusters on LKE 
 Manage nodes and node pools 
 Kubernetes Dashboard on LKE 
 High availability (HA) control plane on LKE 
 Manage a cluster with kubectl 
 Kubernetes versioning and life cycle policy 
 Labels and taints 
 Using GPUs on LKE 
 Upgrade a cluster to a newer Kubernetes version 
 Control Plane ACLs 
 How to drain a node pool on an LKE cluster 
 Rotate Kubernetes secrets 
 Reset kubeconfig 
 Deploy and manage an LKE cluster with the Linode API 
 Load balancing on LKE 
 Secure a cluster with user permissions and RBAC 
 Network and firewall details 
 Create a custom CoreDNS configuration 
 Akamai App Platform (for LKE) Getting Started with the Akamai App Platform 
 Monitor LKE LKE audit logs 
 Metrics for LKE Enterprise 
 Metadata service Add user data when deploying Linodes 
 Access the Metadata service API 
 Use the Metadata service API 
 Use cloud-config files to configure a server 
 Troubleshoot issues with the Metadata service 
 Additional resources 
 Images Capture an image 
 Upload an image 
 Replicate an image 
 Deploy an image to a new Linode 
 Deploy an image to an existing Linode 
 Manage private image sharing (Beta) 
 Object Storage
 Overview 
 Get started with Object Storage Endpoint types 
 Quotas and limits 
 Pricing 
 Get your canonical user ID 
 Create and manage buckets 
 Upload and manage objects 
 Manage access keys 
 Use URLs for access 
 Access and permissions with ACLs 
 Access and permissions with bucket policies 
 Lifecycle policies 
 Clients and tooling AWS CLI and SDKs support 
 Use the Linode CLI with Object Storage 
 Use s3cmd with Object Storage 
 Use s4cmd with Object Storage 
 Use Cyberduck with Object Storage 
 Use the AWS CLI with Object Storage 
 Use the AWS SDK for PHP with Object Storage 
 Use the AWS SDK for Python (boto3) with Object Storage 
 Use Grafana Loki with Object Storage 
 Object Storage use cases Object Storage with the Akamai CDN 
 Custom domain with a TLS/SSL certificate 
 High-throughput applications 
 Data protection Object Lock 
 Versioning 
 Data durability 
 Proper deployment design 
 Default encryption at rest (SSE-S3) 
 Server-side encryption with customer-provided keys (SSE-C) 
 Monitor Object Storage Metrics for Object Storage 
 Logs for Object Storage 
 Cancel Object Storage 
 Other Storage
 Backups Get started with the Backups service 
 Enable backups 
 Schedule backups 
 Take a manual snapshot 
 Restore a backup to a new Linode 
 Restore a backup to an existing Linode 
 Cancel backups 
 Troubleshoot issues with the Backups service 
 Download a local copy of a backup 
 Backups FAQ 
 Block Storage Get started with Block Storage 
 Block Storage quotas 
 View, create, and delete Block Storage volumes 
 Manage Block Storage volumes with the Linode API 
 Volume Encryption 
 Attach and detach a volume 
 Resize a volume 
 Configure and mount a volume 
 Boot from a Block Storage volume 
 Transfer Block Storage data between data centers 
 Transfer a volume to a different Linode 
 Common Block Storage use cases 
 Networking
 Linode Cloud Firewalls Getting started with Cloud Firewalls 
 Create a Cloud Firewall 
 Manage firewall rules 
 Apply firewall rules to a Linode, Linode Interface, or NodeBalancer 
 Update Cloud Firewall status 
 Comparing Cloud Firewalls to Linux firewall software 
 Delete a Cloud Firewall 
 Cloud Firewalls audit logs 
 NodeBalancers Introduction to load balancing 
 Getting started with NodeBalancers 
 Create a NodeBalancer 
 Configuration options for NodeBalancers 
 Using Proxy Protocol with NodeBalancers 
 Available protocols 
 Client's IP address pass-through 
 Backend nodes 
 TLS/SSL termination on NodeBalancers 
 Manage NodeBalancers 
 Monitor NodeBalancers NodeBalancers metrics 
 NodeBalancers audit logs 
 Configure NodeBalancers with the Linode API 
 DNS Manager Getting started with DNS manager 
 Create a domain 
 DNS record types A and AAAA records 
 CNAME records 
 MX records 
 TXT records 
 NS records 
 SOA record 
 CAA records 
 SRV records 
 Manage domains 
 Manage DNS records 
 Configure your domain's authoritative name servers 
 Incoming DNS zone transfers 
 Outgoing DNS zone transfers 
 Troubleshooting DNS records 
 Common DNS configurations 
 VPC Getting started with VPC 
 Create a VPC 
 Manage VPCs 
 Manage VPC subnets 
 Assign a Linode to a VPC 
 Configure a forward proxy to enable internet access within a VPC 
 VPC audit logs 
 VLANs Getting started with VLANs 
 Attach a VLAN to a Linode 
 Detach or delete a VLAN from a Linode 
 Manually configuring a VLAN on a Linode 
 Common use cases for VLANs 
 Create a private network with VLANs using the Linode API 
 Reserved IPs Getting started with reserved IPs 
 Reserve an IP address 
 Manage and assign reserved IPs 
 Databases
 Managed database clusters Get started with managed databases 
 Database engines and plans 
 Create and manage database clusters 
 Advanced configuration parameters 
 Monitor Managed Databases Managed Databases metrics (limited availability) 
 Managed Databases audit logs 
 MySQL 
 PostgreSQL 
 Valkey (limited availability) 
 Monitoring
 Monitor cloud services 
 Monitoring concepts and terminology 
 Metrics (limited availability) Metrics dashboards View metrics for multiple entities 
 View metrics for a single entity 
 Export metrics to external tools Quick start: Metrics export 
 Deployment methods 
 Receiver configuration 
 API rate limits and request batching 
 Hot reload configuration changes 
 Understanding missing metrics 
 Troubleshooting 
 FAQs 
 Metrics reference 
 Alerts (limited availability) Alert types and settings 
 View an alert definition 
 Create a user alert 
 Edit an alert definition 
 Enable or disable an alert 
 Clone an alert 
 Delete an alert 
 Change the monitored entities 
 Notification channels Create a notification channel 
 Manage notification channels 
 Logs Shared responsibilities 
 Get started with logs Quick start: Audit logs 
 Quick start: Kubernetes API audit logs 
 Log streams Create a stream 
 Manage streams 
 Log destinations Create a destination 
 Manage destinations 
 Protect logs in Object Storage 
 Log formats and content 
 Events captured in audit logs 
 Log delivery metrics 
 Longview Get started with Longview 
 View and manage Longview clients 
 System metrics in Longview Capture Apache metrics with Longview 
 Capture NGINX metrics with Longview 
 Capture MySQL metrics with Longview 
 Change Longview plan (upgrade to Pro) 
 Troubleshooting Longview 
 Tools
 Cloud Manager Overview of Cloud Manager 
 Events and activity feeds 
 Tags and groups 
 Search in Cloud Manager 
 Troubleshooting errors in Cloud Manager 
 Linode CLI Get started 
 Administration commands 
 Domains commands 
 Linode instances commands Linode interfaces 
 LKE commands 
 NodeBalancers commands 
 Object Storage commands 
 Support commands 
 Volumes commands 
 StackScripts Get started with StackScripts 
 Create a StackScript 
 Deploy a Linode using a StackScript 
 Manage StackScripts 
 Write a custom script for use with StackScripts 
 Common use cases for StackScripts 
 Use an externally hosted deployment script 
 Object Storage 
 Overview
 ​Akamai​ 's Object Storage is a globally-available, Amazon S3-compatible method you can use to store and access data. It's different from traditional hierarchical data storage, such as a traditional filesystem on a physical or virtual disk or a Block Storage volume . With Object Storage , files (also called objects ) are stored in flat data structures (referred to as buckets ) alongside their own rich metadata.
 With Object Storage , you don't have to use a Linode . Instead, Object Storage gives each object a unique URL that you can use to access it. An object can be publicly accessible, or you can set it to be private, and only visible to you. This makes Object Storage great for sharing and storing unstructured data like images, documents, archives, streaming media assets, and file backups. The amount of data you can store can range from small collections of files to massive libraries of information.
 Features
 Here are some of the features offered with <<Nickname Object Storage :
 Amazon S3-compatible . Object Storage is an Amazon S3-compatible storage solution that supports the use of SDKs, open source projects, and other services built on the Amazon S3 API.
 Global footprint and scale . Object Storage is available in more than 20 regions globally, supporting applications storing petabytes (PB) of content, 100s of thousands of requests per second (RPS), and 100s of Gbps of throughput.
 Strong read-after-write consistency . This ensures data is predictable and minimizes application complexity. With a successful write of a new object or update of an existing one, any subsequent read will receive the latest version, and a listing of the objects in a bucket will accurately reflect the changes.
 Endpoint types
 An endpoint type defines the performance and limits when working with content stored on that endpoint. All endpoints have an assigned type of E0, E1, E2, or E3. To learn more, see Endpoint types .
 Product support and limits
 For detailed information about the limits associated with buckets and each endpoint type, see Quotas and limits .
 Updated 7 days ago 
 Manage private image sharing (Beta)
 Get started with Object Storage
 Did this page help you? Yes 
 No 
 Copy Page 
 Features 
 Endpoint types 
 Product support and limits 
 Legal & privacy Cookie settings Akamai Status 
 Community Training Control Center Cloud Manager 
 © 2026 Akamai Technologies
 Akamai.com 
 Contact us Akamai support Compute support Share feedback 
 Try Akamai 
 Log in Log out 
 Try Akamai 
 Akamai.com 
 Contact us Akamai support Compute support Share feedback 
 Log in 
 Log out
