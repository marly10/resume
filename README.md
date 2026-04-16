# Ricky McKenzie

linkedin.com/in/ricky-mckenzie

---

## Summary

Engineering leader with 7+ years driving observability platform strategy, cloud migrations, and cross-functional team alignment. Currently leading an enterprise migration program (800+ dashboards, 6 teams, 8 GCP projects) and architecting the syslog ingestion pipeline handling 50K+ messages/second into GCP. Early adopter of AI-augmented engineering — built production tooling, automation, and documentation using AI coding assistants to deliver at 3-4x individual capacity. Bilingual (English/Spanish).

---

## Education

**University of San Diego (USD)** — M.S. Engineering Management and Leadership Science | Fall 2025 – Spring 2027

**Point Loma Nazarene University (PLNU)** — B.A. Computer Science, Software Engineering

---

## Experience

### ViaSat Inc — San Diego, CA

**Technical Lead** | Feb 2025 – Present

*Observability Platform Migration:*

- Owned migration strategy for 800+ dashboards across 7 projects, coordinating scope and priorities with 6 teams
- Delivered 34 production dashboards on schedule; established a 5-phase workflow adopted as the standard across all teams
- Triaged 745 dashboards across 3 projects, enabling teams to self-prioritize their backlogs
- Identified infrastructure bottlenecks (200+ TB unclustered data, insufficient compute slots) with data-backed recommendations
- Built an automated status report with live Jira integration, replacing ad-hoc updates across Slack and email
- Reduced conversion cycle time by 95% — one engineer delivering output previously requiring a 3-4 person team

*Bindplane & Syslog Architecture:*

- Architected and documented the syslog ingestion pipeline from ISSRV servers through Bindplane OpenTelemetry collectors into GCP Cloud Logging (50K+ messages/sec in US production)
- Authored wiki documentation for Bindplane architecture, ISSRV integration, and syslog ingestion patterns — used as reference by infrastructure and DevOps teams
- Developed Bindplane routing configurations mapping 5,000+ ISSRV hostnames to correct BigQuery destinations using regex-based YAML rules
- Designed the decommissioning plan for 14 Splunk Universal Forwarder pipelines, transitioning to Bindplane/rsyslog for GCP Cloud Logging (189M events/hour)
- Mapped 68 Databus forwarder streams to BigQuery destinations; automated Confluence wiki updates with contact info and mirroring status

*AI-Augmented Engineering:*

- Used AI coding assistants (Claude Code, GitHub Copilot) to build production tools: migration report generator, query cost analyzer, Jira/Confluence API integrations, Databus forwarder mapping scripts
- Developed AI agent skills and reusable prompts for SQL conversion (Splunk SPL, Snowflake, Druid → BigQuery), schema analysis, and dashboard JSON generation
- Built documentation and conversion agent guides that encode domain knowledge into repeatable AI workflows — reducing onboarding time for future conversions
- Delivered 13,000+ lines of production SQL, a full HTML reporting platform, and Python automation — validated against real data before every deployment

*Team & Process Leadership:*

- Facilitated cross-functional alignment on GCP observability strategy across engineering, operations, and infrastructure teams
- Hired and managed two interns; scoped a Data Platform internship for summer 2025
- Drove evidence-based validation practices and documentation-as-code culture, reducing knowledge silos

*Infrastructure & Cost Optimization:*

- Automated certificate lifecycle management (Ansible/PKI) and AWS certificate signing (Python/ACM API)
- Led transition from Splunk forwarders to OpenTelemetry Agent for GCP Cloud Monitoring
- Analyzed BigQuery slot reservations and Analytics Hub configurations, proposing clustering strategies and compute capacity changes

**DevOps Engineer & Splunk Product Owner (PO)** | Dec 2023 – Jan 2025

- Primary Splunk stakeholder — vendor relationships, license negotiations, quarterly roadmap
- Led platform upgrade across 45 instances (US/EU) with zero unplanned downtime
- Executed storage optimization resulting in **$30K/month AWS cost reduction**
- Delegated daily operations to focus on strategic upgrades and cost reduction

**DevOps Engineer** | April 2022 – Nov 2023

- Led transition from Jenkins/CloudFormation to Terraform-based infrastructure provisioning
- Drove Sensu Classic → Sensu Go migration with team enablement through documentation and pair sessions
- Deployed Splunk infrastructure end-to-end; built reusable Ansible/Python/Bash automation
- Cross-team troubleshooting resource across engineering groups

### Dexcom Inc — San Diego, CA

**System Administrator 1 (Freelance)** | May 2021 – Mar 2022

- Deployed GCP monitoring and patch management across VM fleets using Terraform (InfoSec compliance)
- Automated ISO/SOC2 compliance audit inventory; created self-service Confluence documentation

### The Tides Group — La Jolla, CA

**Software Engineer (Freelance)** | Sep 2019 – May 2021

- Built data collection systems (Java, Python, JavaScript, PHP) and an executive GCP dashboard for the CEO

### Give Back Wireless, Inc. — San Diego, CA

**Mobile Account & Operations Manager** | Feb 2016 – Nov 2020

- Led West Coast business development under AT&T (350+ accounts); managed a team of 6 technicians

---

## Core Competencies

|                           |                                                                                                                           |
| ------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| **Leadership**      | Cross-functional coordination, stakeholder alignment, vendor management, hiring & mentorship                              |
| **AI & Automation** | AI coding assistants (Claude Code, Copilot), AI agent/skill development, prompt engineering, human-in-the-loop validation |
| **Strategy**        | Migration planning, technology roadmaps, cost optimization, risk assessment                                               |
| **Observability**   | BigQuery, Splunk, Grafana, Bindplane/OpenTelemetry, GCP Cloud Logging, Prometheus                                         |
| **Cloud & DevOps**  | GCP (BigQuery, Cloud Logging, Analytics Hub, IAM), AWS (EC2, ACM, IAM), Terraform, Ansible, Python                        |
| **Communication**   | Technical writing (Jira, Confluence, wiki), executive reporting, bilingual (EN/ES)                                        |

---

## Certifications

- Google Cloud Platform Fundamentals
- Essential Google Cloud Infrastructure: Foundation
- Google Cloud Fundamentals: Core Infrastructure
- Solving Infrastructure Challenges with Terraform
- Architecting with Google Kubernetes Engine: Foundations
