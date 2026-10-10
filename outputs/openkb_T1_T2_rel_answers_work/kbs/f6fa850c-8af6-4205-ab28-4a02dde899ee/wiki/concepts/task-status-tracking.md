---
type: "Concept"
sources: ["summaries/session-31_2024-05-15.md"]
description: "A simple method to mark progress of relocation tasks using status dropdowns."
---

# Task Status Tracking

**Definition**: A lightweight approach for indicating the current state of each relocation task, typically using a predefined set of status values (e.g., *Not started*, *In progress*, *Waiting on others*, *Completed*, *Blocked*). The method keeps tracking minimal while providing enough visibility to drive weekly reviews.

## Core Elements
- **Status dropdown**: Implemented via data‑validation in a spreadsheet (e.g., [[entities/google-sheets]]) with the five options above.
- **Column layout**: The sheet includes columns for *Task*, *Category*, *Must‑do/Nice*, *Target Deadline*, *Status*, and *Notes*.
- **Weekly 15‑minute review**: Scan tasks due soon, update statuses, and pick one priority for the next week (as described in [[summaries/session-31_2024-05-15]]).

## How It Supports Relocation Planning
- Fits within the broader [[concepts/relocation-checklist-planning]] by providing a clear progress indicator for each checklist item.
- Aligns with the [[concepts/relocation-timeline-milestones]] framework, allowing users to see which milestones have completed tasks and which still need work.
- Can be combined with a [[concepts/weighted-scoring-method]] when prioritizing tasks, though the basic status tracking remains independent of any scoring.

## Benefits
1. **Low overhead** – Updating a dropdown takes seconds, keeping the 15‑minute weekly maintenance promise.
2. **Immediate visual cue** – Color‑coded or ordered by *Status* makes active items stand out.
3. **Flexibility** – Works in simple notes, Google Sheets, or other list tools without forcing a full project‑management system.

## Implementation Steps (from the session‑31 example)
1. Create a sheet with the column headers mentioned above.
2. Populate rows with tasks and deadlines (see the CSV in [[summaries/session-31_2024-05-15]]).
3. Select the *Status* column, choose **Data → Data validation**, set the dropdown list to the five status options.
4. During each weekly review, filter by upcoming deadlines, update statuses, and reorder by *Status* to keep active work at the top.

---
*Related concepts*: [[concepts/home-selection-checklist]], [[concepts/neighborhood-assessment]]
