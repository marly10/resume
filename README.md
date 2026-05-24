# Ricky McKenzie

619-518-3336 | rickymarly@gmail.com | [linkedin.com/in/ricky-mckenzie](https://linkedin.com/in/ricky-mckenzie) | [github.com/marly10](https://github.com/marly10)

---

## SUMMARY

Bilingual (English/Spanish) Platform Engineer and Technical Lead with 5+ years in DevOps, observability, and cloud infrastructure. Currently leading the migration of 700+ Grafana dashboards from Splunk to BigQuery, building self-service CI/CD pipelines for GCP Cloud Logging, and managing enterprise observability platforms serving 10+ engineering teams. Strong focus on automation, cost optimization, and building tools that eliminate manual work.

---

## EDUCATION

**University of San Diego (USD)** — M.S. Engineering Management and Leadership Science
Fall 2025 – Spring 2027

**Point Loma Nazarene University (PLNU)** — B.A. Computer Science, Software Engineering

---

## EXPERIENCE

### Viasat Inc — Technical Lead, Observability & Platform Engineering
San Diego, CA | Feb 2025 – Present

**Splunk to GCP Migration (OBSRV-1174, OBSRV-1234, OBSRV-1264)**
- Leading migration of 700+ Splunk dashboards across 5 Grafana environments (US, EU, AU), converting SPL, Snowflake SQL, and Druid queries to BigQuery — 78 dashboards and 762 panels converted to date
- Built automated dashboard conversion tooling using Claude Code with 40+ custom skills that handle table mapping, schema validation, variable substitution, and bulk SQL rewriting across 589 dashboards (2,078 panels patched for OBSRV-1253 time filter remediation)
- Designed and executed the Splunk Bindplane UF shutdown plan — validated rsyslog routing conditions against 5,000+ ISSRV hosts across 13 indexes, proving 92-100% data parity with Splunk UF
- Discovered and documented a GCP Cloud Logging log router throughput issue where BQ sinks silently drop 88% of entries when filtering on OTel-transformed labels — created POC sinks with evidence, escalated to Google Cloud support
- Reverse-engineered a 6-bit-per-minute bitmask encoding in BQ dailystats BYTES columns (1080 bytes = 1440 minutes), enabling conversion of a previously "impossible" Splunk panel

**Self-Service Log Router (central_log_sink_router)**
- Built a complete self-service CI/CD system for GCP Cloud Logging log router management — teams define YAML routes, GitHub Actions validates filters against live Cloud Logging, tests IAM, and applies sink changes on merge
- 7 automated workflows: validate → test → apply → drift detection → inventory refresh → PR helpers → auto-generate from issue forms
- Manages log routing across prod and preprod for 14 BQ datasets, with automated PR comments showing filter test results, IAM status, and commit-level change tracking

**BigQuery Cost Analysis Platform (bq-analysis)**
- Built and deployed a Flask web application on Cloud Run (IAP-protected) providing BigQuery inventory, cost analysis, and optimization recommendations across all OBSV-managed GCP projects
- Pages include global inventory, per-team views, dead table detection (zero queries in 60 days), slot monitoring, and GC network migration tracker
- Automated project onboarding pipeline: IAM check → BQ scan → schema pull → storage stats → 60-day jobs snapshot → deploy

**Infrastructure & Operations**
- Automated certificate signing and management for Splunk servers using Ansible playbooks for CSR, private key, and intermediary key management through internal PKI
- Automated AWS Load Balancer certificate signing via the ACM API
- Conducted hiring interviews and managed two interns, including a Data Platform intern (summer 2025)

### Viasat Inc — DevOps Engineer & Splunk Product Owner
San Diego, CA | Dec 2023 – Jan 2025

- Established relationships with Splunk representatives and engineers, negotiated annual Splunk license renewals, defined Jira Epics, and planned quarterly updates
- Delegated daily Splunk maintenance tasks to ensure optimal productivity and momentum
- Upgraded Splunk software from 8.2.5 to 9.0.5 across 45 EC2 instances (US + EU), spanning 7 dev and 38 prod environments
- Created AWS target groups for routing traffic and balancing ingestion across the Splunk ecosystem
- Migrated EC2 volumes from gp2 to gp3, resulting in a $30K/month reduction in AWS costs
- Ensured uptime with Splunk in AZ deployments and conducted general Linux debugging

### Viasat Inc — DevOps Engineer
San Diego, CA | Apr 2022 – Nov 2023

- Deployed general customer enhancements, provided code reviews, deployments via Ansible, and merges for the Sensu Classic to Sensu Go transition
- Developed and deployed infrastructure provisioning with Terraform, replacing Jenkins CI/CD and CloudFormation
- Built Ansible playbooks for all Sensu monitoring components (API, config, event, metric) hosted in AWS — rewrote Ruby scripts to Go
- Developed and deployed automated procedures: cloud-init server provisioning, and scripting with Ansible, Python, and bash for both Sensu and Splunk
- Deployed new Splunk infrastructure: Search Heads, Indexers, Heavy Forwarders, Management servers
- Worked with multiple teams across the company on troubleshooting cross-platform issues

### Dexcom Inc — System Administrator 1 (Freelance)
San Diego, CA | May 2021 – Mar 2022

- Participated in DevSecOps meetings to track task status and align on priorities
- Developed and deployed PowerApps for GCP IAM access policy verification
- Deployed GCP Monitoring Ops Agent across VM clusters (CentOS, Ubuntu, Windows) using Terraform IaC modules
- Deployed GCP VM Manager for OS patch management and InfoSec policy compliance
- Documented processes for VM Manager and Ops Agent management on Atlassian Confluence
- Automated inventory tasks for semi-annual ISO/SOC2 compliance audits

### The Tides Group — Software Engineer (Freelance)
La Jolla, CA | Sep 2019 – May 2021

- Managed, developed, and deployed data collection bots in Java, Python, JavaScript, and PHP for collecting data from websites and APIs
- Deployed GCP-hosted dashboards presenting portfolio health and performance to CEO and executive leadership

### Give Back Wireless, Inc. — Mobile Account & Operations Manager
San Diego, CA | Feb 2016 – Nov 2020

- Business development representative for West Coast region and solution provider under the AT&T umbrella, providing customer service to 350+ customers
- Managed, trained, and scheduled team of 6 triage technicians to ensure product quality and assurance of inventory

---

## TECHNICAL SKILLS

**Languages:** Python, Bash, SQL (BigQuery, Snowflake), Terraform, Ansible, Go, C++, Java

**Cloud Platforms:**
- GCP: BigQuery, Cloud Logging, Cloud Run, IAP, Artifact Registry, Cloud Monitoring, Compute Engine, IAM, Cloud Storage, Analytics Hub
- AWS: EC2, Load Balancer, VPC, Certificate Manager, IAM, Lambda, Billing

**Observability:** Splunk (admin + SPL), Grafana (dashboard development + BQ plugin), Prometheus, Sensu, ELK Stack, Bindplane (OTel collector configuration)

**Infrastructure:** Docker, Kubernetes, GitHub Actions (CI/CD pipeline design), Ansible, Terraform, Linux administration

**Data:** BigQuery (schema design, cost optimization, clustering, INFORMATION_SCHEMA analytics), Snowflake SQL conversion, Druid SQL conversion

**Tools:** Git, GitHub Enterprise, Jira, Confluence (API automation), Claude Code (custom skills + agents)

---

## CERTIFICATIONS

- DevOps Fundamentals — Cloud Academy (2022)
- Docker in Depth — Cloud Academy (2022)
- Essential Google Cloud Infrastructure: Foundation — Coursera (2021)
- Architecting with Google Kubernetes Engine: Foundations — Coursera (2021)
- Google Cloud Fundamentals: Core Infrastructure — Coursera (2021)
- Solving Infrastructure Challenges with Terraform — Cloud Academy (2021)
- Google Cloud Platform Fundamentals — Cloud Academy (2021)

---

## LANGUAGES

- English — Full professional proficiency
- Spanish — Full professional proficiency
