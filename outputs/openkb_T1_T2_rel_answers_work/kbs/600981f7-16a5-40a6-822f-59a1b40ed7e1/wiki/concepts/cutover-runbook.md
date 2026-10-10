---
type: "Concept"
sources: ["summaries/session-12_2025-05-18.md"]
description: "A concise, step‑by‑step guide for executing client migration cutovers."
---

# Cutover Runbook

**Type:** Concept

## Definition
A Cutover Runbook is a short, actionable document that lists the exact commands, links, owners, and timing for each step of a client migration cutover, ensuring a smooth transition and minimal downtime.

## Core Elements (as introduced in [[summaries/session-12_2025-05-18]])
- **Exact commands or links** – Precise CLI commands, API calls, or URLs needed for the cutover.
- **Who runs each step** – Assigned owner or role (e.g., Engineer, On‑call, PM) responsible for executing the step.
- **Expected timing for each step** – Estimated duration or scheduled clock time for each activity.
- **Notes or gotchas** – Quick reminders about prerequisites, rollback triggers, or common pitfalls.

## Typical Structure
```
Cutover runbook:
Exact commands or links: <command / URL>
Who runs each step: <owner or role>
Expected timing for each step: <duration or HH:MM>
Notes or gotchas: <important remarks>
```

## How It Connects to Other Concepts
- It is part of the broader [[concepts/migration-checklist]] that ensures all pre‑cutover items (dependencies, approvals, rollback plan) are completed.
- It fits within a [[concepts/time-blocking]] workflow: the runbook is prepared during the focused migration block and executed during the cutover window.

## Usage Tips
1. **Create the runbook early** – Draft the runbook during the morning focus block so it is ready for validation.
2. **Keep it short** – Aim for no more than a few lines per step; excessive detail slows execution.
3. **Version it** – Store a dated copy (e.g., `clientA‑runbook‑2025‑05‑18.md`) for audit and rollback reference.
4. **Share it** – Post the runbook in a dedicated channel (e.g., `#client‑migration‑runbooks`) before the cutover so all stakeholders have visibility.

---
*This concept page synthesizes the cutover runbook guidance from [[summaries/session-12_2025-05-18]] and places it in the context of related migration practices.*