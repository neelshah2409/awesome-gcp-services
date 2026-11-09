<div align="center">

# Awesome GCP Services [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

**A curated, categorised directory of every major Google Cloud service, built from Google’s official Services Summary.**

[Browse the site](#) · [Recently renamed](#recently-renamed-services) · [Contributing](#contributing)

</div>

> Source of truth: the [Google Cloud Services Summary](https://cloud.google.com/terms/services), the official list of services covered by Google Cloud’s terms, SLAs and support (version last modified **October 21, 2026**). This list was rebuilt against it in **November 2026**. Descriptions are written for this list; follow each link for Google’s own docs.

### Legend

| Marker | Meaning |
| :---: | --- |
| ⚡ | Serverless: no servers or clusters to manage, scales automatically |
| 🆓 | Has a monthly free-tier allowance (limits change; see the [free tier page](https://cloud.google.com/free)) |
| 🔄 | Renamed in 2025–2026; the former name is shown |
| 🔥 | Part of the Firebase platform |
| 📦 | Downloadable software you run yourself |

## Contents

- [Compute](#compute)
- [Serverless](#serverless)
- [Containers & Kubernetes](#containers--kubernetes)
- [Storage](#storage)
- [Databases](#databases)
- [Data & Analytics](#data--analytics)
- [AI, ML & Agents](#ai-ml--agents)
- [Networking](#networking)
- [Security](#security)
- [Identity & Access](#identity--access)
- [Developer Tools & CI/CD](#developer-tools--cicd)
- [Operations & Observability](#operations--observability)
- [API Management & Integration](#api-management--integration)
- [Management & Governance](#management--governance)
- [Migration](#migration)
- [Hybrid, Multicloud & Sovereign](#hybrid-multicloud--sovereign)
- [Firebase](#firebase)
- [Industry Solutions & Media](#industry-solutions--media)
- [Downloadable & Run-Anywhere Software](#downloadable--run-anywhere-software)
- [Recently Renamed Services](#recently-renamed-services)

---

## Compute

- [Compute Engine](https://cloud.google.com/compute) 🆓 - Configurable virtual machines with general-purpose, compute-, memory- and accelerator-optimised machine families. Includes [Cloud GPUs](https://cloud.google.com/gpu), [Cloud TPU](https://cloud.google.com/tpu), Spot VMs, Confidential VMs and sole-tenant nodes.
- [Batch](https://cloud.google.com/batch) - Managed job scheduler that provisions resources, queues and runs batch jobs, then cleans up.
- [Cluster Director](https://cloud.google.com/cluster-director) - Automates setup of large AI and HPC clusters across compute, networking and storage.
- [Google Cloud VMware Engine](https://cloud.google.com/vmware-engine) - Run native VMware workloads in a dedicated private cloud on Google infrastructure.
- [Bare Metal Solution](https://cloud.google.com/bare-metal) - Dedicated bare-metal servers and storage for specialised, low-latency workloads such as Oracle.
- [VM Manager](https://cloud.google.com/compute/docs/vm-manager) - OS patching, inventory and configuration for Windows and Linux VM fleets.
- [Workload Manager](https://cloud.google.com/workload-manager) - Rule-based scans that check workloads (for example SAP) against best practices.
- [License Manager](https://cloud.google.com/compute/docs/license-manager) - Subscribe to and track third-party, per-user licences on Google Cloud.

## Serverless

- [Cloud Run](https://cloud.google.com/run) ⚡🆓 - Run any container as a request-driven **service** or a run-to-completion **job**, scaling to zero.
- [Cloud Run functions](https://cloud.google.com/functions) ⚡🆓🔄 - Event-driven, single-purpose functions (formerly Cloud Functions).
- [App Engine](https://cloud.google.com/appengine) ⚡🆓 - Platform-as-a-service for web applications with no infrastructure to patch.
- [Workflows](https://cloud.google.com/workflows) ⚡🆓 - Orchestrate sequences of Google Cloud services and HTTP APIs.
- [Eventarc](https://cloud.google.com/eventarc) ⚡ - Route events from Google Cloud services and other sources to Cloud Run, functions and Workflows.
- [Cloud Scheduler](https://cloud.google.com/scheduler) ⚡🆓 - Managed cron for HTTP targets, Pub/Sub and App Engine, with retries.
- [Cloud Tasks](https://cloud.google.com/tasks) ⚡🆓 - Distributed task queues for asynchronous, rate-limited work.

## Containers & Kubernetes

- [Google Kubernetes Engine (GKE)](https://cloud.google.com/kubernetes-engine) 🆓 - Managed Kubernetes that provisions, scales and upgrades your clusters.
  - [GKE Autopilot](https://cloud.google.com/kubernetes-engine/docs/concepts/autopilot-overview) ⚡ - Google manages nodes, scaling and security; you pay for pod resources.
  - [Config Sync](https://cloud.google.com/kubernetes-engine/enterprise/config-sync/docs/overview) - GitOps: keep many clusters in sync with configuration under version control.
  - [Policy Controller](https://cloud.google.com/kubernetes-engine/enterprise/policy-controller/docs/overview) - Enforce programmable guardrail policies across clusters and fleets.
  - [GKE Identity Service](https://cloud.google.com/kubernetes-engine/enterprise/identity) - Sign in to clusters with your existing identity provider.
  - GKE Hub and Connect Agent - Register and centrally manage clusters running on Google Cloud, on-prem or other clouds.
- [Cloud Service Mesh](https://cloud.google.com/service-mesh) - Managed mesh with mTLS identity, traffic management and service telemetry.
- [Backup for GKE](https://cloud.google.com/kubernetes-engine/docs/add-on/backup-for-gke/concepts/backup-for-gke) - Back up and restore GKE workloads and their volumes.
- [Binary Authorization](https://cloud.google.com/binary-authorization) - Only allow signed, approved container images to deploy.
- [Artifact Registry](https://cloud.google.com/artifact-registry) 🆓 - Store container images and language packages (see [Developer Tools](#developer-tools--cicd)).

## Storage

- [Cloud Storage](https://cloud.google.com/storage) 🆓 - Object storage with Standard, Nearline, Coldline and Archive classes.
- [Persistent Disk](https://cloud.google.com/persistent-disk) - Durable SSD and HDD block storage for Compute Engine and GKE (with [Hyperdisk](https://cloud.google.com/compute/docs/disks/hyperdisks) for tunable performance).
- [Filestore](https://cloud.google.com/filestore) - Managed NFS file shares for applications that need a shared, POSIX file system.
- [Google Cloud NetApp Volumes](https://cloud.google.com/netapp-volumes) - Managed NetApp ONTAP file storage over NFS, SMB or both.
- [Cloud Managed Lustre](https://cloud.google.com/managed-lustre) - Managed high-performance parallel file system for AI training and HPC.
- [Backup and DR Service](https://cloud.google.com/backup-disaster-recovery) - Centralised, policy-based backup and disaster recovery for Google Cloud workloads.
- [Backup for GKE](https://cloud.google.com/kubernetes-engine/docs/add-on/backup-for-gke/concepts/backup-for-gke) - Data protection for Kubernetes workloads.
- [Cloud Storage for Firebase](https://firebase.google.com/docs/storage) 🔥 - Secure user uploads and downloads for apps, backed by Cloud Storage.

## Databases

- [Cloud SQL](https://cloud.google.com/sql) - Managed MySQL, PostgreSQL and SQL Server.
- [AlloyDB for PostgreSQL](https://cloud.google.com/alloydb) - PostgreSQL-compatible database for demanding transactional and analytical workloads.
- [Spanner](https://cloud.google.com/spanner) - Globally distributed, strongly consistent relational database.
- [Firestore](https://cloud.google.com/firestore) ⚡🆓 - Serverless document database with a MongoDB-compatible API, realtime sync and offline support. Successor to Datastore.
- [Bigtable](https://cloud.google.com/bigtable) - Wide-column NoSQL store for terabyte-to-petabyte, low-latency workloads.
- [Memorystore](https://cloud.google.com/memorystore) - Managed in-memory caching with Valkey, Redis, Redis Cluster and Memcached.
- [Database Migration Service](https://cloud.google.com/database-migration) ⚡ - Minimal-downtime migrations into Google Cloud managed databases.

## Data & Analytics

- [BigQuery](https://cloud.google.com/bigquery) ⚡🆓 - Serverless data warehouse and analytics platform, with built-in ML and AI.
  - [BigQuery Data Transfer Service](https://cloud.google.com/bigquery/docs/dts-introduction) - Scheduled loads from SaaS apps such as Google Ads and YouTube.
  - [BigQuery Omni](https://cloud.google.com/bigquery/docs/omni-introduction) - Query data in other public clouds from BigQuery.
- [Lakehouse](https://cloud.google.com/biglake) 🔄 - Cross-cloud data platform on open storage formats with unified governance (formerly BigLake).
- [Knowledge Catalog](https://cloud.google.com/dataplex) 🔄 - Always-on catalog and knowledge graph that gives agents business context across your data (formerly Dataplex Universal Catalog).
- [Pub/Sub](https://cloud.google.com/pubsub) ⚡🆓 - Global asynchronous messaging between applications.
- [Dataflow](https://cloud.google.com/dataflow) ⚡ - Managed Apache Beam for batch and streaming pipelines.
- [Managed Service for Apache Spark](https://cloud.google.com/dataproc) 🔄 - Managed Spark and Hadoop clusters, plus a serverless option (formerly Dataproc).
- [Dataproc Metastore](https://cloud.google.com/dataproc-metastore) - Managed Apache Hive metastore for open-source data lakes.
- [Managed Service for Apache Airflow](https://cloud.google.com/composer) 🔄 - Managed Airflow for scheduling and monitoring pipelines (formerly Cloud Composer).
- [Google Cloud Managed Service for Apache Kafka](https://cloud.google.com/managed-service-for-apache-kafka) - Managed, open-source-compatible Kafka clusters.
- [Datastream](https://cloud.google.com/datastream) ⚡ - Serverless change data capture and replication.
- [Dataform](https://cloud.google.com/dataform) - Develop, test, version and schedule SQL workflows.
- [Cloud Data Fusion](https://cloud.google.com/data-fusion) - Visual, code-free data integration pipelines.
- [Looker (Google Cloud core)](https://cloud.google.com/looker) - Enterprise BI with a semantic model and embedded analytics.
- [Data Studio](https://cloud.google.com/data-studio) 🔄🆓 - Self-service reports and dashboards (formerly Looker Studio). **Data Studio Pro** adds team governance.
- [Earth Engine](https://cloud.google.com/earth-engine) - Planetary-scale geospatial analysis over satellite imagery.

## AI, ML & Agents

**Platform**

- [Gemini Enterprise Agent Platform](https://cloud.google.com/vertex-ai) 🔄 - Unified platform to build, deploy and govern agents and ML models: datasets, training, pipelines, Model Garden, Workbench and Colab Enterprise (formerly Vertex AI Platform).
  - Generative AI on Gemini Enterprise Agent Platform 🔄 - Gemini API, Live API, Embeddings API, Interactions API and grounding with Google Search, Maps or enterprise web data (formerly Generative AI on Vertex AI).
  - Neural Architecture Search 🔄 - Automatically generate and evaluate model architectures.
  - Gemini Enterprise Agent Platform Vision 🔄 - Build and run computer-vision applications (formerly Vertex AI Vision).
- [Agent Search](https://cloud.google.com/enterprise-search) 🔄 - Semantic search and question answering over your content, with an API and industry editions (formerly Vertex AI Search).
- [Deep Learning VM and Containers](https://cloud.google.com/deep-learning-vm) 📦 - Images preloaded with AI frameworks.

**Agents and assistants**

- [Gemini Enterprise](https://cloud.google.com/gemini-enterprise) - Agents, Gemini models and search connected to company data and apps. Agentspace became part of it in October 2025.
- [Gemini for Google Cloud](https://cloud.google.com/gemini/docs/overview) - AI assistance built into Google Cloud products, including [Gemini Code Assist](https://cloud.google.com/products/gemini/code-assist) and Gemini in BigQuery.
- [NotebookLM Enterprise](https://cloud.google.com/agentspace/notebooklm-enterprise/docs/overview) - Summarise and extract insight from your own documents.
- Computer Use - Lets agents operate a browser, OS or mobile UI from screen input.
- [Firebase AI Logic](https://firebase.google.com/docs/ai-logic) 🔥 - Call generative models securely from mobile and web apps.

**Pre-trained APIs**

- [Cloud Vision API](https://cloud.google.com/vision) 🆓 - Image labelling, object and face detection, and OCR.
- [Video Intelligence API](https://cloud.google.com/video-intelligence) 🆓 - Extract metadata, entities and annotations from video.
- [Speech-to-Text](https://cloud.google.com/speech-to-text) 🆓 - Transcribe audio to text.
- [Text-to-Speech](https://cloud.google.com/text-to-speech) 🆓 - Natural-sounding speech in many voices and languages.
- [Cloud Translation API](https://cloud.google.com/translate) - Text translation with pre-trained or custom models.
- [Cloud Natural Language API](https://cloud.google.com/natural-language) 🆓 - Entities, sentiment, syntax and language detection.
- [Document AI](https://cloud.google.com/document-ai) - OCR, form parsing and custom document extraction and classification.
- [Translation Hub](https://cloud.google.com/translation-hub) - Self-service document translation for organisations.
- [Timeseries Insights API](https://cloud.google.com/timeseries-insights) - Real-time forecasting and anomaly detection over time series.

**Customer experience**

- [Gemini Enterprise for Customer Experience (GECX)](https://cloud.google.com/solutions/customer-engagement-ai) 🔄 - Agents across the customer lifecycle (formerly Customer Engagement Suite / Contact Center AI). Includes CX Agent Studio, Conversational Agents (Flows, formerly Dialogflow CX, and Playbooks), Agent Assist, CX Insights and Contact Center as a Service.
- AI Commerce Search 🔄 - Google-quality product search for retail sites (formerly Vertex AI Search for Commerce).
- [Recommendations AI](https://cloud.google.com/recommendations) - Personalised recommendations from your catalogue and events.

## Networking

- [Virtual Private Cloud (VPC)](https://cloud.google.com/vpc) - Global private networks with IP allocation, routing and firewall policies.
- [Cloud Load Balancing](https://cloud.google.com/load-balancing) - Global and regional L4/L7 load balancing for public and private apps.
- [Cloud CDN](https://cloud.google.com/cdn) - Edge caching for load-balanced content.
- [Media CDN](https://cloud.google.com/media-cdn) - Large-scale streaming and download delivery on Google’s edge.
- [Cloud DNS](https://cloud.google.com/dns) - Managed authoritative DNS.
- [Cloud NAT](https://cloud.google.com/nat) - Managed outbound internet access for private instances.
- [Cloud Interconnect](https://cloud.google.com/network-connectivity/docs/interconnect) - Physical connectivity: Dedicated, Partner, Cross-Cloud and Cross-Site Interconnect.
- [Cloud VPN](https://cloud.google.com/network-connectivity/docs/vpn) - IPsec connectivity with Classic VPN or HA VPN.
- [Cloud Router](https://cloud.google.com/network-connectivity/docs/router) - Dynamic BGP routing between VPC and external networks.
- [Network Connectivity Center](https://cloud.google.com/network-connectivity/docs/network-connectivity-center) - Hub-and-spoke connectivity management, including **NCC Gateway** for securing cross-cloud traffic.
- [Private Service Connect](https://cloud.google.com/vpc/docs/private-service-connect) - Reach managed services privately from inside your VPC.
- [Cloud Next Generation Firewall](https://cloud.google.com/firewall) - Distributed firewall; the Enterprise edition adds intrusion prevention.
- [Cloud IDS](https://cloud.google.com/intrusion-detection-system) - Managed network intrusion detection.
- [Secure Web Proxy](https://cloud.google.com/secure-web-proxy) - Policy control and inspection for workload egress web traffic.
- [Network Security Integration](https://cloud.google.com/network-security-integration) - Insert third-party appliances in-band or out-of-band without re-architecting.
- [Google Cloud Armor](https://cloud.google.com/security/products/armor) - WAF and DDoS defence; **Cloud Armor Enterprise** adds Adaptive Protection and DDoS response support.
- [Network Intelligence Center](https://cloud.google.com/network-intelligence-center) - Network monitoring, verification and optimisation.
- [Cloud Network Insights](https://cloud.google.com/network-intelligence-center/docs/cloud-network-insights) - Performance monitoring for hybrid and cross-cloud networks.
- [Network Service Tiers](https://cloud.google.com/network-tiers) - Choose Premium (Google backbone) or Standard routing.
- [Service Directory](https://cloud.google.com/service-directory) - Publish and discover services across environments.

## Security

- [Security Command Center](https://cloud.google.com/security-command-center) - Centralised posture, vulnerability and threat findings.
- [Cloud Key Management Service](https://cloud.google.com/kms/docs) - Manage cryptographic keys; with [Cloud HSM](https://cloud.google.com/kms/docs/hsm) and [Cloud EKM](https://cloud.google.com/kms/docs/ekm) for hardware-backed and external keys.
- [Key Access Justifications](https://cloud.google.com/assured-workloads/key-access-justifications/docs/overview) - A reason attached to every key request through KMS or EKM.
- [Secret Manager](https://cloud.google.com/secret-manager) 🆓 - Store and version API keys, passwords and certificates.
- [Certificate Manager](https://cloud.google.com/certificate-manager) - Obtain, deploy and track TLS certificates.
- [Certificate Authority Service](https://cloud.google.com/certificate-authority-service) - Managed private certificate authorities.
- [Sensitive Data Protection](https://cloud.google.com/sensitive-data-protection) - Discover, classify and de-identify sensitive data (includes Cloud DLP).
- [VPC Service Controls](https://cloud.google.com/vpc-service-controls) - Security perimeters that reduce data-exfiltration risk.
- [Model Armor](https://cloud.google.com/security-command-center/docs/model-armor-overview) - Screen LLM prompts and responses for injection, data leaks and harmful content.
- [Assured Workloads](https://cloud.google.com/assured-workloads) - Enforced controls for regulated workloads such as FedRAMP.
- [Audit Manager](https://cloud.google.com/audit-manager) - Compliance assessments and audit evidence.
- [Access Transparency](https://cloud.google.com/assured-workloads/access-transparency/docs/overview) - Logs of Google administrator access to your content.
- [Cloud Asset Inventory](https://cloud.google.com/asset-inventory) - Searchable inventory and history of resources and policies.
- [Web Security Scanner](https://cloud.google.com/security-command-center/docs/concepts-web-security-scanner-overview) - Scan web apps for common vulnerabilities.
- [Cyber Insurance Hub](https://cloud.google.com/security/products/cyber-insurance-hub) - Security reports to share with insurers.
- [Google Cloud Fraud Defense](https://cloud.google.com/security/products/recaptcha) 🔄 - Detect fraud and bots on websites (formerly reCAPTCHA Enterprise).
- [Web Risk API](https://cloud.google.com/web-risk) - Check URLs against Google’s lists of unsafe sites.
- [Google Security Operations](https://cloud.google.com/security/products/security-operations) - SIEM and SOAR, covered by the separate [SecOps Services Summary](https://cloud.google.com/terms/secops/services).

## Identity & Access

- [Identity and Access Management (IAM)](https://cloud.google.com/iam) - Who can do what on which resource, including workload identity federation.
- [Identity-Aware Proxy (IAP)](https://cloud.google.com/iap) - Identity-based access to apps and VMs without a VPN.
- [Cloud Identity](https://cloud.google.com/identity) - Users, groups, devices and SSO.
- [Identity Platform](https://cloud.google.com/identity-platform) - Customer identity and sign-in for your own apps.
- [Access Context Manager](https://cloud.google.com/access-context-manager/docs) - Attribute-based access levels for projects and resources.
- [Access Approval](https://cloud.google.com/assured-workloads/access-approval/docs) - Approve Google administrator access before it happens.
- [Chrome Enterprise Premium](https://chromeenterprise.google/products/chrome-enterprise-premium/) - Zero-trust application access and data protection (formerly BeyondCorp Enterprise).
- [Managed Service for Microsoft Active Directory](https://cloud.google.com/managed-microsoft-ad) - Highly available, patched Microsoft AD.

## Developer Tools & CI/CD

- [Cloud Build](https://cloud.google.com/build) ⚡🆓 - Serverless CI that builds from GitHub, Bitbucket or Cloud Storage.
- [Cloud Deploy](https://cloud.google.com/deploy) 🆓 - Managed continuous delivery with promotions and rollbacks.
- [Artifact Registry](https://cloud.google.com/artifact-registry) 🆓 - Container images and language packages.
- [Assured Open Source Software](https://cloud.google.com/security/products/assured-open-source-software) - Google-scanned and fuzz-tested open-source packages.
- [Secure Source Manager](https://cloud.google.com/secure-source-manager/docs/overview) - Fully managed, Git-based source control.
- [Cloud Source Repositories](https://cloud.google.com/source-repositories/docs) - Git version control on Google Cloud.
- [Developer Connect](https://cloud.google.com/developer-connect/docs) - Connect external Git platforms to Google Cloud tools.
- [Cloud Workstations](https://cloud.google.com/workstations) - Managed, secure development environments.
- [Android Device Streaming](https://developer.android.com/studio/run/android-device-streaming) 🔥 - Use remote physical Android devices from Android Studio.
- [Google Device Cloud](https://cloud.google.com/device-cloud) - Remote access to partner-hosted Android devices for testing.
- [Firebase Test Lab](https://firebase.google.com/docs/test-lab) 🔥 - Test mobile apps on many hosted devices.

## Operations & Observability

- [Cloud Monitoring](https://cloud.google.com/monitoring) 🆓 - Metrics, dashboards, uptime checks and alerting.
- [Cloud Logging](https://cloud.google.com/logging) 🆓 - Log ingestion, analysis and routing at scale.
- [Cloud Trace](https://cloud.google.com/trace) 🆓 - Distributed tracing and latency analysis.
- [Cloud Profiler](https://cloud.google.com/profiler) 🆓 - Continuous CPU and memory profiling in production.
- [Error Reporting](https://cloud.google.com/error-reporting) 🆓 - Aggregates application errors and alerts on new ones.
- [Backup and DR Service](https://cloud.google.com/backup-disaster-recovery) - Centralised backup and recovery.
- [Recommender](https://cloud.google.com/recommender/docs) - Cost, security and performance recommendations from your usage.

## API Management & Integration

- [Apigee](https://cloud.google.com/apigee) - Full-lifecycle API management as Apigee X (managed) or Apigee hybrid. **Apigee Edge** remains available too.
- [API Gateway](https://cloud.google.com/api-gateway) ⚡ - Managed gateway for APIs on Google Cloud backends.
- [Cloud Endpoints](https://cloud.google.com/endpoints) - Develop, secure and monitor APIs.
- [Application Integration](https://cloud.google.com/application-integration) - Drag-and-drop iPaaS for connecting apps and data.
- [Integration Connectors](https://cloud.google.com/integration-connectors) - Prebuilt connectors to business apps and data sources.

## Management & Governance

- [Resource Manager](https://cloud.google.com/resource-manager) - Organisations, folders and projects for your resource hierarchy.
- [Organization Policy Service](https://cloud.google.com/resource-manager/docs/organization-policy/overview) - Central guardrails on resource configuration.
- [Infrastructure Manager](https://cloud.google.com/infrastructure-manager/docs) - Managed, declarative infrastructure deployment with Terraform.
- [Cloud Shell](https://cloud.google.com/shell) 🆓 - Browser terminal with the Cloud SDK preinstalled.
- [Cloud Location Finder](https://cloud.google.com/location-finder) - Find regions and zones across Google Cloud, Azure, AWS and OCI by proximity and carbon footprint.
- [Service Infrastructure](https://cloud.google.com/service-infrastructure/docs/overview) - Service Management, Service Control, Service Consumer Management and Service Usage APIs.

## Migration

- [Migration Center](https://cloud.google.com/migration-center) - Discovery, business case, planning and execution for migrations.
- [Migrate to Virtual Machines](https://cloud.google.com/migrate/virtual-machines) - Replication-based VM migration into Compute Engine.
- [Database Migration Service](https://cloud.google.com/database-migration) ⚡ - Minimal-downtime database migrations.
- [Storage Transfer Service](https://cloud.google.com/storage-transfer-service) - Move data from S3, HTTP, NFS or between buckets.
- [Transfer Appliance](https://cloud.google.com/transfer-appliance) - Ship large datasets offline on hardware.
- [BigQuery Data Transfer Service](https://cloud.google.com/bigquery/docs/dts-introduction) - Scheduled SaaS data loads into BigQuery.
- [Migrate to Containers](https://cloud.google.com/migrate/containers/docs) 📦 - Turn VM workloads into containers for GKE and Cloud Run.
- [Kf](https://cloud.google.com/migrate/kf/docs) 📦 - Run Cloud Foundry apps on GKE.

## Hybrid, Multicloud & Sovereign

- [Google Distributed Cloud connected](https://cloud.google.com/distributed-cloud/edge/latest/docs) - Google-managed GKE on dedicated hardware in your premises.
- Google Distributed Cloud connected Appliance - Ruggedised hardware for edge AI and processing in bandwidth-limited sites.
- [Google Distributed Cloud Software-Only](https://cloud.google.com/distributed-cloud) 📦🔄 - Run GKE on your own infrastructure (formerly GKE Enterprise).
- [BigQuery Omni](https://cloud.google.com/bigquery/docs/omni-introduction) - Analyse data in other clouds from BigQuery.
- [Data Boundary by Partners](https://cloud.google.com/terms/in-scope-sovereign-cloud) 🔄 - Sovereign controls with local partners (formerly Sovereign Controls by Partners).
- [Google Cloud VMware Engine](https://cloud.google.com/vmware-engine) and [Bare Metal Solution](https://cloud.google.com/bare-metal) - See [Compute](#compute).

## Firebase

- [Firebase App Hosting](https://firebase.google.com/docs/app-hosting) 🔥⚡ - Serverless full-stack web hosting for Next.js, Angular and more.
- [Cloud Functions for Firebase](https://firebase.google.com/docs/functions) 🔥⚡ - Event-driven backend code for Firebase apps.
- [Firebase Authentication](https://firebase.google.com/docs/auth) 🔥 - User sign-in with email, phone and federated providers.
- [Firebase App Check](https://firebase.google.com/docs/app-check) 🔥 - Attest that API calls come from your genuine app.
- [Firebase Phone Number Verification](https://firebase.google.com/docs/phone-number-verification) 🔥 - One-tap phone number verification via the carrier.
- [Firebase AI Logic](https://firebase.google.com/docs/ai-logic) 🔥 - Generative AI from client apps.
- [Cloud Storage for Firebase](https://firebase.google.com/docs/storage) 🔥 - App file uploads and downloads.
- [Firebase Test Lab](https://firebase.google.com/docs/test-lab) 🔥 - Device testing in the cloud.

## Industry Solutions & Media

- [Cloud Healthcare API](https://cloud.google.com/healthcare-api) - Managed FHIR, HL7v2 and DICOM data.
- [Healthcare Data Engine](https://cloud.google.com/healthcare-data-engine) - Harmonise healthcare data to FHIR and stream it to analytics.
- [Cloud Life Sciences](https://cloud.google.com/life-sciences) - Tools for processing life sciences data.
- [Anti Money Laundering AI](https://cloud.google.com/anti-money-laundering-ai) - AI risk scoring for financial-crime detection.
- [Live Stream API](https://cloud.google.com/livestream) - Cloud live encoding for linear channels and events.
- [Transcoder API](https://cloud.google.com/transcoder) - Batch transcode media into streaming formats.
- [Video Stitcher API](https://cloud.google.com/video-stitcher) - Server-side ad and content insertion.
- [Telecom Network Automation](https://cloud.google.com/telecom-network-automation) - Intent-driven network automation based on Nephio.
- [Spectrum Access System](https://cloud.google.com/spectrum-access-system) - Register and manage CBRS devices in the US 3.5 GHz band.
- [Blockchain Node Engine](https://cloud.google.com/blockchain-node-engine) - Managed node hosting for Web3.
- [Talent Solution](https://cloud.google.com/solutions/talent-solution) - ML-powered job search for career sites and job boards.
- Food Ordering AI Agent - Prebuilt agent for restaurant and drive-thru ordering.
- Automotive AI Agent - Voice-agent framework for in-vehicle experiences.

## Downloadable & Run-Anywhere Software

- [Google Cloud SDK](https://cloud.google.com/sdk) 📦 - `gcloud`, `bq`, `kubectl`, client libraries and local emulators.
- [Config Connector](https://cloud.google.com/config-connector/docs/overview) 📦 - Manage Google Cloud resources as Kubernetes objects.
- [AlloyDB Omni](https://cloud.google.com/alloydb/omni) 📦 - AlloyDB to run in your data centre, any cloud or a laptop.
- [Spanner Omni](https://cloud.google.com/spanner) 📦 - Spanner to run in your own data centre, any cloud or a laptop.
- [Apigee hybrid runtime](https://cloud.google.com/apigee/docs/hybrid/latest/what-is-hybrid) 📦 - Apigee runtime on your Kubernetes.
- [Speech-to-Text On-Prem](https://cloud.google.com/speech-to-text/docs/on-prem) and Cloud Vision OCR On-Prem 📦 - Run Google models in your own environment.
- Telecom Subscriber Insights 📦 - Subscriber engagement insights for telecom operators.
- ABAP SDK for Google Cloud and BigQuery Connector for SAP 📦 - SAP integration with Google Cloud.
- Google Cloud app 📦 - Mobile companion for monitoring and managing resources.

---

## Recently Renamed Services

| Current name | Former name |
| --- | --- |
| Gemini Enterprise Agent Platform | Vertex AI Platform |
| Generative AI on Gemini Enterprise Agent Platform | Generative AI on Vertex AI |
| Agent Search on Gemini Enterprise Agent Platform | Vertex AI Search |
| Gemini Enterprise for Customer Experience | Customer Engagement Suite / Contact Center AI |
| Flows (Conversational Agents) | Dialogflow CX |
| CX Insights | Conversational Insights and Quality AI |
| AI Commerce Search | Vertex AI Search for Commerce |
| Managed Service for Apache Spark | Dataproc |
| Managed Service for Apache Airflow | Cloud Composer |
| Lakehouse | BigLake |
| Knowledge Catalog | Dataplex Universal Catalog |
| Data Studio / Data Studio Pro | Looker Studio / Looker Studio Pro |
| Google Cloud Fraud Defense | reCAPTCHA Enterprise |
| Cloud Run functions | Cloud Functions |
| Google Distributed Cloud Software-Only | GKE Enterprise |
| Google Distributed Cloud connected | Google Distributed Cloud Edge |
| Data Boundary by Partners | Sovereign Controls by Partners |
| Gemini Enterprise (includes Agentspace) | Agentspace |

Product URLs often still use the old names (for example `cloud.google.com/vertex-ai`), so the links above point to the paths Google currently serves.

## Contributing

Contributions are welcome. Please:

1. Check the service against the [official Services Summary](https://cloud.google.com/terms/services) or its product page before adding it.
2. Add it to the most fitting section, in the format `- [Name](link) markers - One-sentence description.`
3. Write descriptions in your own words and keep them to one line.
4. Use the markers from the [legend](#legend) only when they’re accurate.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

This list is released under CC0. Not affiliated with or endorsed by Google. Google Cloud and related names are trademarks of Google LLC.
