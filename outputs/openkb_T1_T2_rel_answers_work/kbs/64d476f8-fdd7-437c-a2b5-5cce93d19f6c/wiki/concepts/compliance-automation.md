---
type: "Concept"
sources: ["summaries/session-07_2025-04-06.md"]
description: "Embedding evidence collection into existing tools to make compliance low‑friction."
---

# Compliance Automation

Compliance Automation is the practice of embedding audit‑ready evidence collection directly into the tools and workflows teams already use, so that compliance data is captured automatically with minimal additional effort.

## Core Principles
- **Leverage existing platforms**: Use the same systems for day‑to‑day work (e.g., IAM, ticketing, CI/CD, cloud logging) as the source of truth for audit artifacts.
- **Automated capture**: Configure logs, timestamps, and required fields to be recorded without manual intervention.
- **Centralized storage**: Push all relevant events to a single repository (commonly a SIEM like [[entities/splunk]]) for easy retrieval.
- **Visibility and predictability**: Provide a shared view of what evidence is required and what is already collected.

## Practical Steps from Session 07 (2025‑04‑06)
1. **Centralize logs** from [[entities/okta]] (identity), [[entities/jira]] (change management), [[entities/github]] / [[entities/github-actions]] (code & deployment), and AWS services ([[entities/aws]]) into Splunk.
2. **Add guardrails** such as required fields or prompts in existing forms to capture missing metadata at the point of action.
3. **Treat evidence as an output** of normal operations – e.g., retain pull‑request merges, deployment logs, and CloudTrail events as the primary audit artifacts.
4. **Expose a dashboard** that shows gaps in real‑time, reducing surprise before a quarterly audit.

## Link to Related Concepts
- The **audit‑bundle** approach (see [[concepts/audit-bundle]]) defines a standardized export package that builds on compliance automation.
- Standardized SPL queries for consistent data extraction are covered in [[concepts/splunk-spl-standardization]].

## Reference Summary
For a full walkthrough of the checklist, audit‑bundle template, and refined SPL queries, see the session summary: [[summaries/session-07_2025-04-06]].