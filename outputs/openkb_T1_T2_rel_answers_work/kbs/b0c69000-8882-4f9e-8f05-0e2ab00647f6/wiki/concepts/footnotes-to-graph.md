---
type: "Concept"
sources: ["summaries/session-10_2024-07-15.md"]
description: "A lightweight layer adding context to visible code contributions."
---

# Footnotes to the Contribution Graph

**Definition**: A concise, human‑generated layer that records work not captured by public contribution graphs (e.g., GitHub or GitLab), providing context without duplicating visible activity.

## Purpose
- Complements automatic logs from platforms like [[entities/github]] and [[entities/gitlab]].
- Captures invisible effort such as private repo work, architecture decisions, mentoring, experiments, and documentation.
- Keeps the overall work record honest, readable, and easy to maintain.

## Core Principles
1. **Narrative over scoreboard** – Treat the footnotes as a running story that explains *why* work mattered, not *how many* commits were made. See [[concepts/activity-tracking]].
2. **No duplication** – Exclude anything already visible on the contribution graph (commits, PRs, timestamps, metrics). Focus on outcomes, decisions, and impact.
3. **Lightweight format** – Use a simple Markdown template (see [[concepts/template-design]]) updated monthly or quarterly.

## Typical Content
- **Private Work Highlights**: High‑level summaries of work in private repositories, e.g., service reliability improvements or internal tooling.
- **Non‑Code Contributions**: Architecture discussions, design docs, mentorship, incident response, research, or any activity that doesn’t produce code artifacts. See [[concepts/non-code-contributions]].
- **Context Not Reflected on GitHub**: Brief notes on constraints, decision rationale, or experimental outcomes that have no commit trace.

## Relationship to Other Concepts
- Acts as a *footnote* layer to the automatic logs discussed in [[concepts/activity-tracking]].
- Relies on the structured approach defined in [[concepts/template-design]].
- Provides the non‑code perspective highlighted in [[concepts/non-code-contributions]].

## Example Usage
The template recommended in [[summaries/session-10_2024-07-15]] includes sections for private work, non‑code contributions, and future notes. By populating those sections each quarter, developers maintain a clear, non‑redundant record that can be shared in performance reviews or team updates.

## Benefits
- **Clarity**: Stakeholders see both visible code output and the hidden effort behind it.
- **Efficiency**: Minimal time required; just a few bullet points per period.
- **Trustworthiness**: Avoids the perception of bragging by focusing on impact, not volume.

---
*This concept page was derived from the discussion in [[summaries/session-10_2024-07-15]].*