---
type: "Concept"
sources: ["summaries/session-07_2025-04-06.md"]
description: "A structured export package of compliance evidence for quarterly audits."
---

# Audit Bundle

**Definition**: An Audit Bundle is a predefined collection of log exports and evidence artifacts, packaged with consistent naming conventions and time‑range rules, to streamline quarterly compliance reviews.

## Purpose
The bundle reduces manual effort by automating the extraction of required data from core systems and presenting it in a predictable, audit‑ready format. It aligns with the principles of [[concepts/compliance-automation]] by embedding evidence collection into existing workflows.

## Core Components
| Component | Export File | Typical Source | Key Fields |
|-----------|------------|----------------|-----------|
| Identity & Access | `Okta_IAM_QX_YYYY.json` | [[entities/okta]] System Log | timestamp, eventType, actor, target, outcome |
| Change Management | `Jira_Changes_QX_YYYY.csv` | [[entities/jira]] tickets | issue key, summary, reporter, assignee, created, resolved, approval status |
| CI/CD Deployments | `CICD_Deploys_QX_YYYY.zip` | [[entities/github]] & [[entities/github-actions]] runs | run ID, commit SHA, artifact hashes, conclusion |
| Infrastructure & Application Logs | `InfraApp_Logs_QX_YYYY.zip` | [[entities/aws]] CloudTrail & CloudWatch | eventTime, eventName, userIdentity, requestParameters, logStream, message |
| Security Controls | `Security_Controls_QX_YYYY.zip` | Various scanners feeding into [[entities/splunk]] | host, severity, detection type, backup job status |

## Naming Convention
- **QX** – quarter number (e.g., Q1, Q2)
- **YYYY** – year
- Prefix indicates the source (e.g., `Okta`, `Jira`, `CICD`).

## Standardized SPL Queries
The bundle relies on a set of repeatable Splunk SPL statements (see [[concepts/splunk-spl-standardization]]) that enforce:
1. Consistent **START/END** variables for the quarter plus a 7‑day buffer.
2. Fixed `table` field lists for each export.
3. Normalization of multivalue fields using `mvexpand`/`mvjoin` where needed.

## Typical Workflow
1. **Set time window** – define `START` and `END` for the target quarter.
2. **Run SPL queries** – execute the standardized searches for each source.
3. **Export** – save results using the naming convention.
4. **Bundle** – compress related files into a single ZIP per category.
5. **Validate** – verify that required fields are present and that file hashes match expected values.

## Benefits
- **Predictability** – identical outputs each quarter, easing auditor review.
- **Low friction** – no manual data hunting; everything is pulled from existing logs.
- **Traceability** – each artifact includes immutable timestamps and source identifiers.
- **Gap detection** – missing files or fields immediately surface during validation.

## Reference
For the original discussion that defined this concept, see [[summaries/session-07_2025-04-06]].