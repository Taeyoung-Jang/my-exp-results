---
type: "Concept"
sources: ["summaries/session-36_2024-06-15.md", "summaries/session-01_2022-06-15.md"]
description: "Sprint planning method that isolates large work into sequential, trackable milestones."
---

# Milestone‑Based Sprint Planning

**Definition**: A sprint planning technique that breaks a large initiative into a series of concrete milestones, pulls only the next milestone into the sprint backlog, and caps the initiative’s capacity to keep it from dominating the sprint.

---

## Core Principles
1. **Separate Track** – Treat the large initiative as its own *track* that runs alongside regular sprint work. [[concepts/migration-track]]
2. **Milestone Granularity** – Decompose the initiative into small, meaningful milestones (e.g., contract validation, data‑mapping, cutover planning). [[concepts/milestone-based-sprint-planning]]
3. **Pull‑Only‑Next Milestone** – At sprint start, commit only to the immediate next milestone; subsequent milestones stay visible but are not promised.
4. **Capacity Capping** – Reserve a fixed portion of the team’s capacity (e.g., 12‑15 story points out of a 40‑point sprint) for the migration track. [[concepts/capacity-capping]]
5. **Visible Progress** – Use stand‑up checkpoints like *current → next → blocked?* to keep the work transparent.

---

## Step‑by‑Step Application (as illustrated in [[summaries/session-01_2022-06-15]])
1. **Identify the big initiative** (e.g., a client integration migration).
2. **Define the milestone sequence**:
   - Milestone 1: Validate new API contract & data mapping.
   - Milestone 2: Draft full migration plan (mapping appendix, cutover playbook, risk summary).
   - Milestone 3: Rehearse cutover in staging.
3. **Select the current milestone** for the sprint (e.g., Milestone 2 when the focus is finalizing the migration plan).
4. **Create backlog items** that deliver the artifacts required for that milestone, each with a clear *Definition of Done*.
5. **Set a capacity cap** for the migration track (≈30 % of total sprint capacity).
6. **Track progress** daily and only move to the next milestone once the current one is completed and signed off.

---

## Benefits
- **Focus**: Teams work on a well‑bounded piece of work, reducing scope creep.
- **Predictability**: Milestones give clear checkpoints and measurable outcomes.
- **Visibility**: The larger initiative remains on the radar without overwhelming the sprint.
- **Risk Management**: Early validation of each milestone surfaces blockers early.

---

## Related Concepts
- [[concepts/migration-track]] – the broader idea of handling large migrations as an independent work stream.
- [[concepts/capacity-capping]] – the practice of limiting how much of the sprint capacity the migration track can consume.

---

*This concept page synthesizes guidance from the session‑01 sprint planning discussion dated 2022‑06‑15.*

See also: [[summaries/session-36_2024-06-15]]