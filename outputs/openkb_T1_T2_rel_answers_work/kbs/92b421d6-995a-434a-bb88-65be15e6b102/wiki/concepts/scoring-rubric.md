---
type: "Concept"
sources: ["summaries/session-36_2024-12-15.md", "summaries/session-15_2023-06-15.md"]
description: "A 0‑2 per‑pillar metric that rates migration test results on editability, metadata, and output fidelity."
---

# Scoring Rubric

The **Scoring Rubric** is a lightweight evaluation framework introduced in the [[summaries/session-15_2023-06-15]] to help decide whether a migration path is viable. It breaks the assessment of each pilot project into three core pillars:

1. **Reopen/Editability** – how cleanly the exported or converted file opens in the target software.
2. **Metadata Preservation** – whether critical project metadata survives the export/conversion.
3. **Final Output Fidelity** – how closely the regenerated output matches the original.

Each pillar receives a score of **0, 1, or 2**:

| Pillar | 2 – Full | 1 – Partial | 0 – Fail |
|--------|----------|--------------|----------|
| Reopen/Editability | Opens cleanly with full structure intact | Opens but with noticeable breakage that can be fixed | Cannot open or too broken to salvage |
| Metadata Preservation | All important fields preserved correctly | Some fields lost but non‑critical | Critical metadata missing or wrong |
| Final Output Fidelity | Visually identical or trivially different | Small differences but still acceptable | Noticeable quality loss or incorrect output |

The three pillar scores are summed to produce a **total score out of 6**. The rubric is used during the [[concepts/pilot-testing]] phase to quantify the success of each export method.

## Interpreting the Total Score
- **5–6** – Indicates a reliable migration path; the method can be applied to the full set of projects.
- **3–4** – Borderline; migration may be possible if cleanup is easy and repeatable.
- **0–2** – Not viable without major tooling or a different strategy.

These thresholds feed directly into the broader [[concepts/migration-planning]] decision rule, where a certain percentage of projects must achieve a high score before committing to a full migration.

---
*This concept page synthesizes the scoring approach from the session‑15 discussion and connects it to related migration planning concepts.*

See also: [[summaries/session-36_2024-12-15]]