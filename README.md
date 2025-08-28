# 🚀 GCP Mastery Bootcamp — 30 Days (README)

Intensive **8–10 hrs/day** bootcamp to compress a 120-day mastery plan into **30 days**.  
Build real projects, practice daily, and prep for **ACE / Professional** certifications.

---

## 📌 How to Use This Repo
- Check off each day’s tasks (`[x]`) as you finish.
- Log what you learned in **Daily Progress**.
- Keep all lab code in `/labs/<day>/` and project code in `/projects/`.

---

## 🗓️ Day-by-Day Plan

### Week 1 — Core Foundation (Days 1–7)
> Focus: Org/project setup, IAM, VPC, compute, storage, load balancing, security.

- [ ] **Day 1 – Org & IAM Fundamentals**
  - Read: GCP resource hierarchy, billing, projects
  - Lab: Create project, enable billing, budget alerts
  - Lab: Create service accounts, grant least-privilege roles
- [ ] **Day 2 – VPC Deep Dive**
  - Read: VPC, subnets, routes, firewall rules, Shared VPC
  - Lab: Custom VPC with 2 subnets; firewall to allow SSH from your IP only
- [ ] **Day 3 – Cloud Storage**
  - Read: Storage classes, lifecycle, versioning, signed URLs
  - Lab: Static website on Cloud Storage with policy-only access
- [ ] **Day 4 – Compute Engine**
  - Read: Instance types, disks, images, instance templates, MIG
  - Lab: Instance template + Managed Instance Group + health checks
- [ ] **Day 5 – Load Balancing & Cloud DNS**
  - Read: HTTP(S), TCP/UDP, internal LBs; Cloud DNS zones/records
  - Lab: HTTPS LB with backend MIG + Cloud DNS A record
- [ ] **Day 6 – Security Essentials**
  - Read: IAM policies, Org Policies, Cloud KMS, Secret Manager
  - Lab: Encrypt app secrets with KMS + Secret Manager; rotate keys
- [ ] **Day 7 – Mini Project A**
  - Deliverable: 2-tier app (VM API + DB) behind HTTPS LB, IAM-secured ops
  - Add architecture diagram + README in `/projects/mini-project-a/`

---

### Week 2 — Data & Serverless (Days 8–14)
> Focus: Databases, BigQuery, Pub/Sub, Cloud Functions, Cloud Run, APIs, caching.

- [ ] **Day 8 – Relational & NoSQL**
  - Read: Cloud SQL (MySQL/Postgres), Firestore modes, Spanner overview
  - Lab: Cloud SQL instance + private IP; connect from VM via IAM DB Auth
- [ ] **Day 9 – BigQuery Basics**
  - Read: Datasets/tables, partitions, cost controls
  - Lab: Ingest CSV from GCS; write queries; scheduled queries
- [ ] **Day 10 – Pub/Sub & Dataflow Intro**
  - Read: Topics, subscriptions, push/pull, DLQs; Dataflow overview
  - Lab: Pub/Sub → Cloud Function subscriber; ack/retry patterns
- [ ] **Day 11 – Cloud Functions & Cloud Run**
  - Read: Event-driven vs request-driven, revisions, concurrency
  - Lab: Deploy containerized API to Cloud Run with min/max instances
- [ ] **Day 12 – API Gateway / Apigee**
  - Read: API authentication (API keys, IAM), quotas
  - Lab: Front Cloud Run with API Gateway; protect with API key + IAM
- [ ] **Day 13 – Memorystore & Cloud Tasks**
  - Read: Redis caching, queues, idempotency
  - Lab: Add Redis cache to Cloud Run API; async jobs with Cloud Tasks
- [ ] **Day 14 – Mini Project B**
  - Pipeline: GCS upload → Pub/Sub → Cloud Function → BigQuery
  - Observability: add logs/metrics/dashboards
  - Commit docs and IaC to `/projects/mini-project-b/`

---

### Week 3 — DevOps, Containers & IaC (Days 15–21)
> Focus: GKE, CI/CD, monitoring, Terraform, service mesh.

- [ ] **Day 15 – Kubernetes on GCP (GKE)**
  - Read: Nodes, pods, services, Ingress, Workload Identity
  - Lab: Cluster + NGINX deployment + Ingress; use Workload Identity
- [ ] **Day 16 – Scaling & Config**
  - Read: HPA/VPA, PodDisruptionBudgets, ConfigMaps/Secrets
  - Lab: HPA based on CPU; PDB for zero-downtime deploys
- [ ] **Day 17 – CI/CD with Cloud Build**
  - Read: Triggers, substitutions, Artifact Registry
  - Lab: Build & push image → deploy to GKE automatically on Git push
- [ ] **Day 18 – Terraform on GCP**
  - Read: Providers, state, modules, environments
  - Lab: Provision VPC + GKE + Cloud SQL via Terraform modules
- [ ] **Day 19 – Cloud Monitoring & Logging**
  - Read: Uptime checks, SLOs, alerting policies, log-based metrics
  - Lab: Dashboards + alerts (latency, error rate, saturation)
- [ ] **Day 20 – Service Mesh (Istio/Anthos Intro)**
  - Read: Sidecars, mTLS, traffic splitting, retries/timeouts
  - Lab: Canary 90/10 → 50/50 rollout with retries + timeouts
- [ ] **Day 21 – Mini Project C**
  - Deliverable: GitHub → Cloud Build → GKE CI/CD + dashboards + alerts
  - Docs: runbook + SLO/SLA in `/projects/mini-project-c/`

---

### Week 4 — Advanced Networking, Security & Capstone (Days 22–30)
> Focus: hybrid networking, WAF, DR, cost controls, ML/analytics, final build.

- [ ] **Day 22 – Hybrid Connectivity**
  - Read: Cloud VPN, Interconnect, VPC peering, Private Service Connect
  - Lab: Simulate site-to-site VPN between two VPCs; Private access to SQL
- [ ] **Day 23 – Security Hardening**
  - Read: Security Command Center, Cloud Armor (WAF), Binary Authorization
  - Lab: WAF rules for L7 protection; Binary Auth for signed images only
- [ ] **Day 24 – Dataflow & Dataproc**
  - Read: Batch/stream pipelines, Spark/Hadoop on Dataproc
  - Lab: ETL job (GCS → Dataflow → BigQuery) + sample Spark job on Dataproc
- [ ] **Day 25 – Vertex AI**
  - Read: Datasets, training, endpoints, AutoML vs custom
  - Lab: Train & deploy a simple model; call from Cloud Run API
- [ ] **Day 26 – FinOps & Budgets**
  - Read: Committed use discounts, rightsizing, labels, cost allocation
  - Lab: Budgets/alerts + BigQuery cost views + Looker Studio dashboard
- [ ] **Day 27 – DR & Backups**
  - Read: RPO/RTO, multi-region, backups/snapshots, HA patterns
  - Lab: Simulate region failure; validate restore & failover docs
- [ ] **Days 28–29 – Capstone Project**
  - Build: **E-commerce microservices**
    - Frontend: Cloud Run
    - Backend: GKE (services, Ingress, HPA)
    - DB: Cloud SQL (private IP)
    - Events: Pub/Sub (orders/payments)
    - Analytics: Dataflow → BigQuery → Looker dashboard
    - Sec: Cloud Armor, IAM, Secret Manager, Binary Auth
    - IaC: Terraform modules for all stacks
    - SRE: SLOs, alerts, runbooks, cost dashboard
  - Deliverables: Architecture diagram, README, deploy scripts
- [ ] **Day 30 – Mastery Check & Cert Prep**
  - Mock exams: ACE + Professional (Architect/DevOps)
  - Fill gaps; finalize docs; publish portfolio write-up

---

## 🧪 Daily Study Template (Copy into `/progress/`)
```md
## Day X (YYYY-MM-DD)
**Focus:** <topic>
**Study:** <docs/videos/courses>
**Labs:** <hands-on tasks and results>
**Issues & Fixes:** <troubleshooting notes>
**Key Takeaways:** <bullets>
**Next Up:** <plan>

