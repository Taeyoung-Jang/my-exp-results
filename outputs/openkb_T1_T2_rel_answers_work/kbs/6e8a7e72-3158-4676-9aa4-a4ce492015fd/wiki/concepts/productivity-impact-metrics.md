---
type: "Concept"
sources: ["summaries/session-10_2024-07-15.md"]
description: "Metrics for measuring how premium features affect personal productivity."
---

# Productivity Impact Metrics

**Definition**: A set of simple, repeatable measurements used to assess whether a premium subscription tangibly improves efficiency, quality, or outcomes compared to a baseline workflow.

## Core Metrics Introduced in [[summaries/session-10_2024-07-15]]

1. **Frequency of Use** – Count how many times per day/week a premium feature is invoked. A high frequency suggests potential impact, but must be qualified by outcome.
2. **Time Difference** – Estimate the time the task would have taken without the feature versus the actual time with it. Record as minutes saved or added.
3. **Outcome Quality** – Subjective rating of the result (e.g., *better*, *slightly worse*, *no change*) or a concrete quality score if applicable.
4. **Irritation vs. Real Loss** – Note moments of habit‑driven annoyance separate from measurable slowdown. Use a simple tag like `irritation` or `real‑impact`.
5. **Fallback Usage** – Log any emergency reinstatement of the premium tool during the test; this indicates critical dependence.

## Simple Scoring Scheme

- **No Change** – Tasks feel the same, time difference negligible, quality unchanged.
- **Slightly Worse** – Minor increase in time or small dip in quality; may still be acceptable.
- **Significantly Worse** – Noticeable slowdown (≥ 10‑15 % longer) or clear quality degradation.

Summarize the week by counting how many days fall into each category. A predominance of *No Change* or isolated irritation spikes points to a *nice‑to‑have* feature, whereas consistent *Slightly/Significantly Worse* results signal genuine value.

## Relationship to Other Concepts

- The metrics support the broader framework of [[concepts/premium-value-assessment]], providing the quantitative side of the evaluation.
- They are applied during a [[concepts/trial-off-experiments]] such as the “avoid‑premium week” described in the source document.
- The entity at the center of this assessment is often a [[entities/premium-subscription]].

## Practical Template (excerpt)

```
Date: YYYY‑MM‑DD
Task: … (normally uses premium feature)
Time w/feature: X min | Time w/out: Y min
Quality: better / same / worse
Impact tag: [irritation | real‑impact]
Notes: …
```

Use this template daily, then aggregate the scores at the end of the test period to decide whether the premium subscription remains worthwhile.
