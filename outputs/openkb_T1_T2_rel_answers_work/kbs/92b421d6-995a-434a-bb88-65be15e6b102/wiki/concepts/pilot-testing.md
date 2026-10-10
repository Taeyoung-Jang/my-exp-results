---
type: "Concept"
sources: ["summaries/session-36_2024-12-15.md", "summaries/session-15_2023-06-15.md"]
description: "A short‑term, representative test to evaluate migration feasibility."
---

# Pilot Testing

**Definition**

Pilot testing is a lightweight, weekend‑scale trial that uses a small, representative set of legacy projects to assess whether a migration path to new software is realistic.

**Purpose**

- Validate export and conversion options identified in [[concepts/migration-planning]].
- Gather empirical data on editability, metadata preservation, and output fidelity.
- Provide a concrete basis for scoring each method using the [[concepts/scoring-rubric]].

**Typical Workflow**

1. **Select Representative Projects** – Choose 3‑4 projects covering simple, typical, and complex cases (the minimum recommended number).  
2. **Run Export/Conversion Methods** – Apply each native export option and any third‑party converters, saving results in clearly labeled folders.
3. **Log Findings** – Use a structured log template (see the session summary) to record reopen success, broken elements, metadata gaps, output differences, time spent, and a confidence score.
4. **Score Each Project** – Apply the three‑pillar rubric (editability, metadata, output) to obtain a 0‑6 score per project.
5. **Aggregate Results** – Fill a summary sheet that averages scores, notes common failures, and estimates cleanup effort.
6. **Decision Rule** – If at least 60‑70 % of projects score ≥5 and none fall below 3, the method is deemed a viable full migration; otherwise consider a hybrid approach.

**Key Benefits**

- **Risk Reduction** – Detect deal‑breaking issues before committing to a full migration.
- **Quantitative Evidence** – Scores and time metrics provide objective criteria for decision‑making.
- **Scalability Insight** – Estimate the effort required to migrate all ~50 legacy projects based on the pilot workload.

**Relation to Other Concepts**

Pilot testing directly supports [[concepts/migration-planning]] by supplying the empirical data needed to choose an export strategy, and it utilizes the [[concepts/scoring-rubric]] to turn qualitative observations into actionable scores.

**Source**

The procedure is derived from the checklist and templates outlined in [[summaries/session-15_2023-06-15]].

See also: [[summaries/session-36_2024-12-15]]