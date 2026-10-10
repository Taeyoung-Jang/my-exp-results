---
type: "Concept"
sources: ["summaries/session-36_2024-12-15.md", "summaries/session-15_2023-06-15.md"]
description: "Framework for evaluating software migration feasibility via testing, scoring, and decision rules."
---

# Migration Planning

**Migration Planning** is the systematic process of deciding whether to stay with a legacy software platform or move to an alternative, based on concrete evidence rather than intuition. It combines **export and conversion analysis**, a limited **pilot testing** effort, and a quantitative **scoring rubric** to produce a clear go‑/no‑go decision.

---

## Core Elements

1. **Export & Conversion Review**
   - Identify all native export formats the current software supports.
   - Survey third‑party conversion tools or compatibility layers.
   - Document tool versions, settings, and output locations.

2. **Pilot Testing** – a weekend‑scale trial using a small, representative set of projects (see [[concepts/pilot-testing]]). The pilot captures real‑world behavior of export, conversion, and re‑opening in the target platform.

3. **Scoring Rubric** – each test project is scored on three pillars (editability, metadata preservation, output fidelity) using a 0‑2 scale, yielding a total score out of 6 (see [[concepts/scoring-rubric]]). The rubric provides an objective measure of migration viability.

4. **Decision Rule**
   - **Full Migration**: ≥ 60 % of pilot projects score 5 or 6 and none score below 3.
   - **Hybrid**: Mixed results where some projects achieve high scores while others fall short; retain the legacy tool for the problematic cases and archive them in a neutral format.
   - **No Migration**: Majority of scores ≤ 2 or cleanup effort exceeds a reasonable threshold.

5. **Hybrid Strategy**
   - Keep the legacy software available for legacy‑only projects.
   - Export and archive those projects in the most stable neutral format.
   - Migrate only the high‑scoring projects, using the documented workflow.

---

## Workflow Summary

1. **Select Representative Projects** – simple, typical, and complex (minimum three).
2. **Run All Export/Conversion Methods** – save each result in a labeled folder.
3. **Log Results** – use the Project Log Template from the source.
4. **Apply Scoring Rubric** – assign scores for editability, metadata, and output.
5. **Compile Summary Sheet** – aggregate scores, note common failures/successes, and compute averages.
6. **Make Decision** – apply the decision rule to choose migration, hybrid, or stay‑put.

---

## Relation to Source Document

The detailed checklist, log template, scoring rubric, and decision thresholds are derived directly from the discussion in [[summaries/session-15_2023-06-15]], which presents a pragmatic weekend‑pilot plan for evaluating a migration path.

---

### References
- [[concepts/pilot-testing]]
- [[concepts/scoring-rubric]]
- [[summaries/session-15_2023-06-15]]

See also: [[summaries/session-36_2024-12-15]]