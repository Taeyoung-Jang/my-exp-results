---
type: "Concept"
sources: ["summaries/session-40_2024-06-15.md", "summaries/session-14_2022-06-15.md"]
description: "A lightweight single‑page system for tracking weekly client projects and actions."
---

# One‑Page Weekly Dashboard

A **One‑Page Weekly Dashboard** is a minimal‑overhead visual board that lets a designer keep track of active client projects, deadlines, and the next concrete action for each project—all on a single page. It is designed to avoid the complexity of full‑blown project‑management tools while still providing enough structure to prevent work from slipping through the cracks.

## Core Elements

1. **Project List** – One line per client/project.
2. **Key fields per line**:
   - **Current Deliverable** – What is being produced right now.
   - **Deadline** – Exact date (or date‑time) the deliverable is due.
   - **Next Action** – The single next step the designer will take.
   - **Parking Lot (optional)** – Brief list of low‑priority items.
3. **Status Columns** – Simple three‑column layout:
   - **This Week** – Projects that need attention this week.
   - **Waiting/Feedback** – Items awaiting client input.
   - **Done** – Completed tasks for quick visual closure.

## Implementation Examples

- **Trello**: Create a board with the three lists above. Each card follows the template shown in [[summaries/session-14_2022-06-15]] and uses the **card template** to capture the fields.
- **Notion**: Build a database named “Weekly Projects” (see [[entities/notion]]). Add properties: *Name*, *Deadline* (Date), *Priority* (Select), *Current Deliverable* (Text), *Next Action* (Text). View it as a table or kanban board.

## How It Supports the Weekly Rhythm

The dashboard aligns with the **deep‑work** mornings described in [[concepts/deep_work]] by surfacing the *primary* project for the day at a glance. It also dovetails with the **triage rule** ([[concepts/triage_rule]]): any request that does not belong on the dashboard can be quickly categorized as non‑urgent and placed in the afternoon queue.

## Benefits

- **Visibility**: All active projects and their most important next step are visible at a glance.
- **Low friction**: Updating a single line takes seconds, encouraging frequent refreshes.
- **Flexibility**: Works in both [[entities/trello]] and [[entities/notion]] (or any note‑taking app).
- **Focus**: By limiting information to the essential three fields, the dashboard prevents overwhelm and supports the weekly schedule from the source document.

## Usage Tips

- Review the dashboard each morning to pick the **primary project** based on deadline, impact, and creative load.
- At the end of the day, move completed items to **Done** and add any new tasks to the **Parking Lot**.
- Schedule a brief Friday review to ensure all upcoming deadlines are captured and the next week's priorities are set.


See also: [[summaries/session-40_2024-06-15]]