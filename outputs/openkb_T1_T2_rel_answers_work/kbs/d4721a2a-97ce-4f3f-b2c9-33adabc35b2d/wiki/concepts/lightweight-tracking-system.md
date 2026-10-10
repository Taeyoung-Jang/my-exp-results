---
type: "Concept"
sources: ["summaries/session-34_2024-12-14.md"]
description: "A minimal, tool‑based method for tracking owners and pending items using Outlook, Teams, and OneNote."
---

# Lightweight Tracking System

A **lightweight tracking system** is a deliberately simple workflow that lets knowledge workers keep tabs on who owns which responsibilities and what they are waiting on, without turning the process into a separate project management tool. The design focuses on leveraging existing productivity platforms—**Outlook**, **Teams**, and **OneNote**—and on habit‑based upkeep so the system stays useful with a few seconds of daily effort.

## Core Principles
- **Minimal data** – only four essential fields: Name, Ownership, What I’m waiting on, Last touchpoint.
- **Single source of truth** – a single OneNote page hosts the master table, keeping search fast and avoiding duplication.
- **Tool‑native cues** – Outlook categories (Owner, Waiting, FYI) and a saved search folder surface urgent items without extra software.
- **Regular micro‑maintenance** – a 30‑second capture routine and a 10‑minute daily sweep keep the list current.

## Recommended Setup
1. **OneNote page** – create a page titled *People + Ownership* with two headings:
   - **Who owns what** – the main table (Name, Domain/Ownership, What I’m waiting on, Last touchpoint).
   - **Active waiting items** – a small area where you paste rows you need to act on this week.
2. **Outlook categories** – set up three categories:
   - *Owner* (blue)
   - *Waiting* (orange)
   - *FYI* (green)
3. **Outlook search folder** – *Waiting this week* filters messages tagged Waiting and received within the last 7 days.
4. **Teams habit** – pin a chat per active workstream and add a brief note that mirrors the OneNote row when new context arrives.

## Maintenance Checklists
- **30‑second capture** (see [[concepts/quick-capture-checklist]])
  - Add name
  - Add ownership phrase
  - Add "what I need" phrase + date
- **10‑minute daily sweep** (see [[concepts/minimum-viable-workflow]])
  - Clean aged or resolved rows
  - Move top priorities to *Active waiting items*
  - Park stale rows (see [[concepts/workplace-boundaries]] for a simple rule: move to *Parked* after ~14 days of no activity)

## Example Rows (copy‑paste ready)
```
Alex R. | Vendor contracts | Waiting on updated SOW for Q2 | 3/12 – draft coming this week
Priya T. | Build pipeline dependency | Need status on blocker (looped in by Sam) | 3/14 – replied in Teams thread
```

## Scaling the System
- When the table exceeds ~30 people, add a collapsible **Inactive / Parked** section below the active rows.
- Archive whole parked blocks monthly to a new OneNote page (e.g., *Archive – March*), preserving history without clutter.

## Benefits
- **Speed** – all actions fit into the gaps between meetings.
- **Visibility** – quick lookup of ownership via OneNote search or Outlook’s Waiting view.
- **Low friction** – no dedicated project‑management software required; it works inside the tools you already use.

---
**Related concepts**: [[concepts/minimum-viable-workflow]], [[concepts/quick-capture-checklist]], [[concepts/workplace-boundaries]]

**Source**: [[summaries/session-34_2024-12-14]]