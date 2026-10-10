---
type: "Concept"
sources: ["summaries/session-01_2022-06-15.md"]
description: "A method for isolating a large migration initiative as a dedicated track within a sprint."
---

# Migration Track

**Definition**
A _migration track_ is a lightweight, parallel workflow used to manage a big, moving‑parts migration project without letting it dominate the regular sprint backlog. It treats the migration as its own “track” that runs alongside normal sprint work.

**Origin**
The concept is introduced in [[summaries/session-01_2022-06-15]], where the assistant recommends handling a messy migration‑style initiative as a separate track.

**Key Characteristics**
- **Isolation:** The migration work is scoped and scheduled separately from feature stories, keeping the core sprint focused.
- **Milestone‑driven:** Only the next concrete milestone is pulled into the sprint, following the [[concepts/milestone-based-sprint-planning]] approach.
- **Capacity‑capped:** The team explicitly limits the effort allocated to the migration track, typically 30 % of total capacity, as described in [[concepts/capacity-capping]].
- **Visibility:** Progress is tracked with simple stand‑up checks (current → next → blocked?) to keep stakeholders aware without overwhelming the board.

**Typical Workflow**
1. **Identify the overall migration goal** (e.g., client integration, data model change).
2. **Break the goal into discrete milestones** that deliver a tangible, reviewable outcome.
3. **Select the next milestone** as the current focus and pull only the work needed to achieve it into the sprint backlog.
4. **Allocate a capped capacity** (e.g., 12‑15 story points) for the migration track.
5. **Track progress** during daily stand‑ups and update the migration board or a dedicated column in [[entities/jira]].
6. **Upon completion**, mark the milestone done, update the migration plan in [[entities/confluence]], and move to the subsequent milestone in the next sprint.

**Benefits**
- Prevents the migration from swallowing the entire sprint.
- Provides clear, incremental delivery points.
- Improves risk visibility and enables early detection of blockers.
- Keeps regular delivery cadence intact while still advancing the larger initiative.

**Related Concepts**
- [[concepts/milestone-based-sprint-planning]] – the practice of organizing work around concrete milestones.
- [[concepts/capacity-capping]] – the technique of reserving a fixed portion of sprint capacity for special work.

---
*This page synthesizes the approach described in the source session and serves as a reusable pattern for agile teams facing large migration projects.*