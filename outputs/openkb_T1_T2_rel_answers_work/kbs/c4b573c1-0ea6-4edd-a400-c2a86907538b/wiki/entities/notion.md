---
sources: ["summaries/session-38_2024-12-16.md"]
type: "Product"
description: "A flexible workspace and note‑taking tool used to build lightweight dashboards."
---

# Notion

**Type:** product

Notion is a collaborative workspace platform that combines notes, databases, and project‑tracking features in a single interface. In [[summaries/session-38_2024-12-16]] it is recommended as the host for the **lightweight dashboard** that helps teams achieve rapid [[concepts/team-alignment]] and manage [[concepts/handoff-risk-management]].

## Key facts from the session
- **Use case:** Build a single‑page priorities board (a [[concepts/lightweight-dashboard]]) to surface active projects, owners, priorities, next handoffs, dates, and a health signal.
- **Implementation details:**
  - Create a table with columns: Project, Owner, Collaborator, Priority, Phase, Next Handoff, Handoff Date, What’s Needed Next, Health.
  - Leverage Notion’s built‑in *Last Edited* property to detect “no progress” (unchanged for 7 days).
  - Configure multiple views (upcoming hand‑offs, priority overload per Owner, stalled work) that can be filtered and sorted without extra tooling.
- **Benefits:**
  - Provides a shared, low‑maintenance view that supports asynchronous weekly updates.
  - Keeps the process lightweight (≈ 1 minute to edit) while still exposing handoff risks and priority conflicts.
- **Stakeholders mentioned:** [[entities/maya]], [[entities/jordan]], [[entities/lena]], [[entities/ravi]], [[entities/chris]] – all can edit or view the Notion page according to their role.

## Related concepts
- [[concepts/lightweight-dashboard]] – the design pattern the Notion table follows.
- [[concepts/team-alignment]] – the broader goal of creating shared visibility.
- [[concepts/handoff-risk-management]] – the specific risk the dashboard surface.

## Practical tips for Notion users
1. **Set permissions** so owners can edit their rows while others have read‑only access.
2. **Use the default "Table – Full page"** view for the master sheet; add filtered views for each stakeholder group.
3. **Enable the "Last edited time" column** to automatically track inactivity for the “no progress” rule.
4. **Schedule a weekly async check‑in** (e.g., every Monday 9 am) where each owner updates their row before the summary is posted.
