---
type: "Concept"
sources: ["summaries/session-07_2025-04-06.md"]
description: "Standardized Splunk SPL queries for consistent audit data extraction."
---

# Splunk SPL Standardization

**Definition**: A set of best‑practice Splunk Search Processing Language (SPL) patterns that ensure audit‑related data is extracted, normalized, and presented consistently across quarterly compliance runs.

## Why it matters
In [[concepts/compliance-automation]] programs, evidence must be collected automatically from sources such as [[entities/okta]], [[entities/jira]], [[entities/github]], [[entities/github-actions]], and AWS services ([[entities/cloudtrail]], [[entities/cloudwatch]]).  Without a unified SPL approach, teams end up with fragmented exports, missing fields, and ambiguous formats that increase manual effort and audit risk.

## Core elements
1. **Uniform time window** – All queries use `earliest=START latest=END` placeholders so the same quarterly range (plus optional buffer) applies everywhere.
2. **Explicit field selection** – The `table` command lists a stable column set, guaranteeing downstream processing can rely on fixed headers.
3. **Multivalue normalization** – Arrays that arrive as multivalue fields are flattened using `mvexpand` and recombined with `mvjoin` to produce a single‑line record per event (e.g., reviewers in GitHub PR merges).
4. **Placeholder customization** – Custom Jira approval fields or other organization‑specific attributes are represented as clearly marked placeholders (e.g., `CUSTOM_APPROVAL_FIELD`) that can be swapped without altering the query logic.
5. **Naming conventions** – Export files follow the pattern used in the [[concepts/audit-bundle]] (e.g., `Okta_IAM_QX_YYYY.json`), reinforcing traceability between the query output and the audit bundle.

## Example queries (from [[summaries/session-07_2025-04-06]])
- **Okta identity logs** – Pulls authentication, group, and policy events and outputs a fixed set of columns.
- **GitHub PR merges** – Uses `mvjoin` to flatten `requested_reviewers` and `reviews` multivalue fields before tabling.
- **Jira change‑type issues** – Filters on issue type and a placeholder approval field, then tables the essential metadata.
- **AWS CloudTrail** – Limits to high‑value services (`ec2`, `iam`, `s3`, `cloudformation`) and selects core attributes.
- **GitHub Actions workflow runs** – Captures run identifiers, outcomes, and job status in a repeatable table.

These queries reside in a shared library that the compliance team can call from a scripted runbook, ensuring every quarter the same data shape is produced.

## Benefits
- **Reduced manual effort** – Teams run a single script rather than crafting ad‑hoc searches.
- **Audit‑ready output** – Consistent column order and naming match the audit‑bundle templates, simplifying packaging.
- **Error‑proofing** – Normalizing multivalue fields eliminates ambiguous “array” cells that Splunk otherwise returns.
- **Scalability** – New sources can adopt the same pattern (time window, `table`, `mvexpand`/`mvjoin`) without reinventing the wheel.

---
*This concept is derived from the discussion in [[summaries/session-07_2025-04-06]] and ties into the broader compliance‑automation framework.*