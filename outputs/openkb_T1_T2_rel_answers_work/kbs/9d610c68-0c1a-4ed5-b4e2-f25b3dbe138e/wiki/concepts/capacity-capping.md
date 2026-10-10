---
type: "Concept"
sources: ["summaries/session-36_2024-06-15.md", "summaries/session-01_2022-06-15.md"]
description: "Allocating a fixed portion of sprint capacity to a large migration track to protect regular work flow."
---

# Capacity Capping

**Type:** Concept

**Description:** A technique for reserving a predefined share of a sprint’s total capacity for a large, cross‑cutting initiative (e.g., a migration) so that it remains visible but does not dominate the sprint.

## Why It Matters
In multi‑team or product environments, big migration or infrastructure projects can easily consume all available story points, causing the sprint to lose focus on its primary deliverables. By explicitly capping the effort—often expressed in story points or hours—the team safeguards the regular backlog while still making measurable progress on the larger effort.

## How It Is Applied (from [[summaries/session-01_2022-06-15]])
1. **Determine total sprint capacity** – e.g., 40 story points.
2. **Set a cap for the migration track** – the session recommends 12‑15 story points (≈30 % of capacity).
3. **Allocate only that amount to migration tasks** – backlog items such as contract validation, mapping, or draft migration plan are scoped to fit within the cap.
4. **Track remaining capacity** – the rest of the sprint (≈25‑28 story points) is used for regular feature work.
5. **Review at sprint end** – if the migration track finishes early, extra capacity can be borrowed; if it overruns, the team learns and adjusts the cap for the next sprint.

## Relationship to Other Concepts
- **[[concepts/migration-track]]** – Capacity capping is applied specifically to a dedicated migration track, ensuring it runs alongside normal work.
- **[[concepts/milestone-based-sprint-planning]]** – Coupled with milestone‑based planning, the capped capacity focuses the team on completing one concrete milestone per sprint.

## Benefits
- Prevents a large initiative from swallowing the sprint.
- Increases predictability for both the migration and regular work.
- Improves visibility: the migration track appears in the sprint board, but its size is bounded.
- Facilitates smoother hand‑offs between milestones, as each sprint has a clear, limited goal.

## Risks & Mitigations
| Risk | Mitigation |
|------|------------|
| Under‑estimating migration effort → cap too low | Re‑evaluate after each sprint; adjust the cap based on actual velocity.
| Over‑allocating migration work → regular backlog suffers | Keep a strict review of sprint goal and enforce the cap during sprint planning.

## Example from the Source Session
> "Keep the migration work capped at about 12 to 15 story points out of the team’s 40‑point capacity so the initiative is controlled without consuming the full sprint."

This concrete recommendation illustrates how capacity capping can be operationalized in a real sprint.


See also: [[summaries/session-36_2024-06-15]]