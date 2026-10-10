---
type: "Concept"
sources: ["summaries/session-12_2025-05-18.md"]
description: "A reusable, structured checklist for managing client migration tasks end‑to‑end."
---

# Migration Checklist

**Definition**: A reusable, structured list of items that ensures all critical steps of a client migration are completed, reviewed, and documented.

## Core Components (from [[summaries/session-12_2025-05-18]])

1. **Dependencies** – Verify that all required systems, data, and services are ready before starting the migration.  
2. **Approvals** – Capture who has signed off and track the status of each required approval.  
3. **Rollback Plan** – Confirm a tested rollback strategy is documented and ready to execute if needed.  
4. **Cutover Steps** – List the exact commands, links, and responsible owners for each step of the cutover.  
5. **Validation Checks** – Define post‑cutover verification tasks to confirm the migration succeeded.  
6. **Go/No‑Go Criteria** – Include explicit checkboxes for stakeholder sign‑off and on‑call support coverage.  
7. **Communications** – Prepare draft messages or notifications to be sent to stakeholders and end‑users.  
8. **Risks & Open Questions** – Record any outstanding concerns that could affect the migration.  
9. **Next Action & Owner** – Assign the immediate follow‑up task and responsible person.

## Checklist Template (copy‑paste ready)
```
Client name:
Dependencies confirmed: [ ]
Approvals received: [ ]
Rollback plan updated: [ ]
Cutover steps ready: [ ]
Validation checks defined: [ ]
Go/no‑go readiness:
  Stakeholder sign‑off received: [ ]
  Support / on‑call coverage confirmed: [ ]
  All blockers cleared: [ ]
Comms drafted or queued: [ ]
Risks or open questions:
Next action and owner:

Cutover runbook:
Exact commands or links:
Who runs each step:
Expected timing for each step:
Notes or gotchas:
```

## Related Concepts
- [[concepts/time-blocking]] – scheduling technique that protects dedicated migration windows.
- [[concepts/cutover-runbook]] – detailed step‑by‑step guidance for the cutover phase.
- [[concepts/migration-checklist]] – this very concept; see also the source summary for context.

---
*This concept page distills the migration checklist presented in the session‑12 summary, offering a reusable artifact for future client migrations.*