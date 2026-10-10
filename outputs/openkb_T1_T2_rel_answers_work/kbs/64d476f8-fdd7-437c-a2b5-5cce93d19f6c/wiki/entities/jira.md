---
sources: ["summaries/session-07_2025-04-06.md"]
type: "Product"
description: "Jira is a product for issue tracking and change management."
---

# Jira

**Type:** Product  
**Description:** Issue tracking and change management platform used for compliance evidence.

## Role in Session 7 (2025‑04‑06)
- Serves as the central system for recording change‑type issues (e.g., Change, Normal, Emergency) and their approvals.
- Exported for audit‑bundle generation via Splunk SPL targeting the `index=jira` dataset.
- The SPL query normalizes custom approval fields (placeholders) and filters by issue type, supporting the [[concepts/audit-bundle]] workflow.
- Integrated with other tools such as [[entities/github]] for code merges and [[entities/okta]] for IAM evidence, forming a low‑friction compliance pipeline described in [[concepts/compliance-automation]].

## Key Facts from the Document
- Export format: CSV named `Jira_Changes_QX_YYYY.csv`.
- Required fields in the SPL export: `_time`, `issue.key`, `issue.summary`, `issue.reporter`, `issue.assignee`, `issue.created`, `issue.updated`, `issue.resolutiondate`, `issue.type`, custom approval fields (`CUSTOM_APPROVAL_FIELD`, `CUSTOM_APPROVER_FIELD`), and `issue.status`.
- Used together with other sources like [[entities/aws]] (CloudTrail), [[entities/github-actions]], and [[entities/splunk]] to create a comprehensive quarterly audit package.

## Links
- Related concepts: [[concepts/compliance-automation]], [[concepts/audit-bundle]], [[concepts/splunk-spl-standardization]]
- Related entities: [[entities/okta]], [[entities/github]], [[entities/aws]], [[entities/splunk]]
- See the summary of the session that introduced this information: [[summaries/session-07_2025-04-06]]