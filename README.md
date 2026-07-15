# Ricky McKenzie

### Senior Platform Engineer | Observability Lead | AIOps & AI-Assisted Engineering

619-518-3336 | rickymarly@gmail.com | [linkedin.com/in/ricky-mckenzie](https://linkedin.com/in/ricky-mckenzie) | [github.com/marly10](https://github.com/marly10)

---

## SUMMARY

Bilingual (English/Spanish) Senior Platform Engineer and Technical Lead with 6+ years in DevOps, observability, and cloud infrastructure. Owns the organization-wide GCP logging roadmap at Viasat, defining centralized and decentralized logging standards across 1,000+ GCP projects and driving architectural decisions adopted by engineering teams and leadership. Currently leading the migration of 700+ Grafana dashboards from Splunk to BigQuery, designing and operating OpenTelemetry (OTel) log collection pipelines via Bindplane at 5,000+ host scale, and building self-service CI/CD platforms for GCP Cloud Logging. Strong track record of turning complex, manual engineering problems into automated, scalable systems.

---

## KEY IMPACT

- **1,000+ GCP projects** under centralized logging governance and roadmap ownership
- **700+ dashboards migrated** across 5 Grafana environments (US, EU, AU); 2,078 panels bulk-remediated in a single automated pass
- **5,000+ hosts** running through the production OTel/Bindplane log pipeline across US and EU
- **18 anomaly detectors** deployed to production; 100+ candidates in development
- **~$210K/month** modeled savings from org-wide log exclusion strategy at scale
- **$30K/month** AWS cost reduction from infrastructure optimization in prior role

---

## EDUCATION

**University of San Diego (USD)** — M.S. Engineering Management and Leadership Science
Fall 2025 – Spring 2027 (in progress)

**Point Loma Nazarene University (PLNU)** — B.A. Computer Science, Software Engineering

---

## EXPERIENCE

### Viasat Inc — Technical Lead, Observability & Platform Engineering

San Diego, CA | Feb 2025 – Present

**GCP Logging Architecture & Strategy**

- Serves as Viasat's internal logging platform lead — owns the organization-wide GCP logging roadmap, defines centralized and decentralized logging standards across 1,000+ GCP projects, and authors architectural designs adopted by engineering teams and platform leadership
- Designed the org-scale centralized logging architecture end-to-end: org-level aggregating sink auto-capturing all GCP projects, three regional log buckets (US/EU/AU), per-team scoped Log Views, BigQuery Linked Datasets, and per-team Authorized Views — built on a non-intercepting sink model that preserves local team alerting while enabling cross-org analytics, cost attribution, and unified log search
- Authored the internal logging reference guide defining how teams access centralized logs (Log Scope, Log Analytics, direct BigQuery SQL) and the data governance model for scoped access at org scale; presented architecture to engineering leadership and cross-functional stakeholders

**Splunk → BigQuery Migration & Automation**

- Leading migration of 700+ Splunk dashboards across 5 Grafana environments (US, EU, AU), converting SPL, Snowflake SQL, and Druid queries to BigQuery — 78 dashboards and 762 panels completed; bulk-remediated 2,078 panels across 589 dashboards for a time-filter compliance issue
- Built automated conversion tooling using Claude Code with 40+ custom agentic skills handling table mapping, schema validation, variable substitution, and bulk SQL rewriting — reducing week-long manual work to hours per dashboard

**OpenTelemetry Log Pipeline**

- Designed and operated a production Bindplane OpenTelemetry (OTel) log collection pipeline replacing Splunk Universal Forwarder — RFC5424 syslog → Bindplane OTel Gateway → GCP Cloud Logging → 14 BigQuery datasets; 5,000+ ISSRV hosts across 6 log indexes in US and EU prod
- Managed Bindplane OTel collector configurations end-to-end — receivers, processors, and exporters for syslog ingestion; translated Splunk host routing patterns to RE2 log router filters for GCP Cloud Logging, including discovery and fix of systematic regex failures silently dropping EU hosts
- Validated 92–100% data parity across 12 log indexes with a 3-way benchmark (Splunk vs OTel rsyslog pipeline vs legacy Splunk UF pipeline) and a custom 5-tier host classification system before decommissioning the legacy forwarder fleet

**Self-Service Log Routing CI/CD**

- Built a GitOps-based self-service system for GCP Cloud Logging log router management — teams define YAML routes, 7 GitHub Actions workflows validate filters against live Cloud Logging, test IAM, detect drift, and apply sink changes on merge; manages routing across prod and preprod for 14 BigQuery datasets
- Handles the full lifecycle: filter validation, IAM verification, diff-based PR comments showing exactly what changes, automated inventory refresh, and issue-form-driven onboarding

**Engineering Analytics Platform & Tooling**

- Deployed a live BigQuery analytics web application (Cloud Run, IAP-protected) serving the engineering org with BigQuery inventory, cost analysis, dead table detection, slot monitoring, and migration tracking across all observability-managed GCP projects — functions as a living engineering portfolio and decision-support tool for platform leadership
- Modeled log ingestion exclusion impact at org scale — simulated 70% exclusion filter coverage across a 400-project organization; identified ~$210K/month in potential Cloud Logging ingestion cost reduction; findings adopted by platform leadership to set exclusion filter targets and prioritize cost reduction initiatives
- Automated project onboarding from days to hours: IAM check → BQ scan → schema pull → storage stats → 60-day query history snapshot → deploy; Ansible automation for PKI certificate management (Splunk servers) and AWS ACM certificate signing
- Conducted hiring interviews and managed two interns, including a Data Platform intern (summer 2025)

**AIOps: Anomaly Detection & Alerting Platform**

- Built and deployed a containerized BigQuery-powered anomaly detection system monitoring 6 log datasets — 18 detectors running continuously in production, surfacing threshold breaches, behavioral anomalies, and correlated failure patterns as structured Slack alerts with plain-English descriptions, affected host samples, and confidence scores
- Designed the alert output standard to be immediately actionable: every alert leads with a one-line plain-English summary, includes raw counts and affected terminal IDs as evidence, and states confidence explicitly; GCS-backed audit trail captures all detector outputs for replay and review
- Managing a pipeline of 100 candidate detectors (50 standalone log-signal detectors + 50 enriched detectors combining log signals with correlation data); phased promotion to production as each candidate is validated against real incident history

### Viasat Inc — DevOps Engineer & Splunk Product Owner

San Diego, CA | Dec 2023 – Jan 2025

- Owned the Splunk enterprise platform as sole technical product lead — managed vendor relationships, negotiated annual license renewals, and drove quarterly roadmap planning for a platform serving 10+ engineering teams across US and EU
- Led a major Splunk version upgrade (8.2.5 → 9.0.5) across 45 EC2 instances (7 dev + 38 prod, US + EU), coordinating across teams while maintaining platform availability
- Reduced AWS infrastructure costs by $30K/month through EC2 volume migration (gp2 → gp3) and optimized target group routing for Splunk ingestion workloads
- Maintained high-availability Splunk deployments (AZ-distributed Search Heads, Indexers, and Heavy Forwarders) and resolved cross-platform incidents across engineering teams

### Viasat Inc — DevOps Engineer

San Diego, CA | Apr 2022 – Nov 2023

- Deployed general customer enhancements, provided code reviews, deployments via Ansible, and merges for the Sensu Classic to Sensu Go transition
- Developed and deployed infrastructure provisioning with Terraform, replacing Jenkins CI/CD and CloudFormation
- Built Ansible playbooks for all Sensu monitoring components (API, config, event, metric) hosted in AWS — rewrote Ruby scripts to Go
- Developed and deployed automated procedures: cloud-init server provisioning, and scripting with Ansible, Python, and bash for both Sensu and Splunk
- Deployed new Splunk infrastructure: Search Heads, Indexers, Heavy Forwarders, Management servers
- Worked with multiple teams across the company on troubleshooting cross-platform issues

### Dexcom Inc — System Administrator 1 

San Diego, CA | May 2021 – Mar 2022

- Participated in DevSecOps meetings to track task status and align on priorities
- Developed and deployed PowerApps for GCP IAM access policy verification
- Deployed GCP Monitoring Ops Agent across VM clusters (CentOS, Ubuntu, Windows) using Terraform IaC modules
- Deployed GCP VM Manager for OS patch management and InfoSec policy compliance
- Documented processes for VM Manager and Ops Agent management on Atlassian Confluence
- Automated inventory tasks for semi-annual ISO/SOC2 compliance audits

### The Tides Group — Software Engineer 

La Jolla, CA | Sep 2019 – May 2021

- Managed, developed, and deployed data collection bots in Java, Python, JavaScript, and PHP for collecting data from websites and APIs
- Deployed GCP-hosted dashboards presenting portfolio health and performance to CEO and executive leadership

### Give Back Wireless, Inc. — Operations Manager

San Diego, CA | Feb 2016 – Nov 2020

- Managed, hired, trained, and scheduled a team of 6 technicians — responsible for performance management, product quality assurance, and day-to-day operations
- Grew West Coast regional sales as an AT&T umbrella partner, providing account management for 350+ customers

---

## TECHNICAL SKILLS

**Languages:** Python, Bash, SQL (BigQuery, Snowflake), Terraform, Ansible, Go, C++, Java

**Cloud Platforms:**

- GCP: BigQuery, Cloud Logging, Cloud Run, IAP, Artifact Registry, Cloud Monitoring, Compute Engine, IAM, Cloud Storage, Analytics Hub
- AWS: EC2, Load Balancer, VPC, Certificate Manager, IAM, Lambda, Billing

**Observability:** Splunk (admin + SPL), Grafana (dashboard development + BQ plugin), Prometheus, Sensu, ELK Stack

**OpenTelemetry (OTel):** Bindplane pipeline design (receivers, processors, exporters), OTel log data model & semantic conventions, collector configuration & deployment, GCP Cloud Logging OTel integration, log router sink management, high-throughput pipeline troubleshooting

**Infrastructure:** Docker, GitHub Actions (CI/CD pipeline design), Ansible, Terraform, Linux administration

**Data:** BigQuery (schema design, cost optimization, clustering, INFORMATION_SCHEMA analytics), Snowflake SQL conversion, Druid SQL conversion

**AIOps & AI-Assisted Engineering:** Production anomaly detection and automated alerting pipeline design (threshold + behavioral detectors), custom skill and agent authoring across Claude (Claude Code, subagents, skills) and ChatGPT (custom GPTs, prompt engineering), multi-agent automation pipeline design, AI-assisted engineering workflows

**Tools:** Git, GitHub Enterprise, Jira, Confluence (API automation), Claude Code (40+ custom agentic skills)

---

## LANGUAGES

- English — Full professional proficiency
- Spanish — Full professional proficiency
