---
type: "Concept"
sources: ["summaries/session-38_2024-12-16.md"]
description: "A minimal, single‑page view that surfaces priorities, handoffs, and health signals."
---

# Lightweight Dashboard

**Definition** – A concise, single‑page artifact (often a spreadsheet or Notion table) that shows only the most actionable signals needed for team alignment without adding process overhead.

## Core Purpose
- Provide a shared, real‑time view of what work is active, what is coming next, and where handoffs occur.
- Surface **[[concepts/handoff-risk-management]]** by flagging upcoming transitions that could become bottlenecks.
- Support **[[concepts/team-alignment]]** through a quick, asynchronous update rhythm rather than additional meetings.

## Key Elements (as described in [[summaries/session-38_2024-12-16]])
| Column | Description |
|---|---|
| **Project** | Name of the initiative. |
| **Owner** | Primary responsible person. |
| **Collaborator** | Secondary person (if any). |
| **Priority** | High / Medium / Low – a lightweight tag to avoid debate. |
| **Phase** | Current stage (e.g., Design Review, In Progress). |
| **Next Handoff** | The next transition point (e.g., Engineering kickoff). |
| **Handoff Date** | Expected date for that transition. |
| **What’s Needed Next** | Short note of the immediate requirement. |
| **Health** | Traffic‑light status (Green, Yellow, Red) tied to timing and blockage. |

### Health Signal Rules
- **Green** – Handoff date realistic; no blockers.
- **Yellow** – Date at risk because something is waiting on another person or an open question exists.
- **Red** – Date will be missed unless something changes; work is blocked or shows **no progress** (the “What’s Needed Next” field unchanged for 7 days).

## Views for Rapid Insight
1. **Upcoming Hand‑offs** – Sorted by *Handoff Date* to see what’s approaching.
2. **Conflicting Priorities** – Filter by *Owner* and highlight multiple *High* items.
3. **Stuck Work** – Show rows where *Health* is Red **or** the “What’s Needed Next” field hasn’t changed in a week.

## Review Cadence
- **Weekly async check‑in**: each owner updates their row before a set time (e.g., Monday 9 am).
- After updates, a brief written summary notes any red items or overlapping high‑priority handoffs.
- No extra synchronous meeting is required unless a red item demands immediate discussion.

## Benefits
- **Speed** – Takes ~1 minute to update, encouraging consistent use.
- **Transparency** – Everyone can glance at the board to understand current focus and risks.
- **Low overhead** – Avoids turning the artifact into a full‑blown project‑management system.

---
*Related concepts*: [[concepts/team-alignment]], [[concepts/handoff-risk-management]]
