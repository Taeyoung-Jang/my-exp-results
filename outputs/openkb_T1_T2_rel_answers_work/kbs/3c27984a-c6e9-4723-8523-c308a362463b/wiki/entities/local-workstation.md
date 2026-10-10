---
sources: ["summaries/session-13_2024-06-15.md"]
type: "Product"
description: "A $10k compute‑heavy workstation used for simulation workloads."
---

# Local Workstation

A high‑performance workstation or server, typically costing around $10,000, equipped with a powerful CPU and optionally a GPU, intended for running compute‑heavy simulations locally.

## Key Facts from session‑13_2024‑06‑15
- **Cost basis**: $10k purchase price amortized over three years (~$3,300/yr).
- **Power & cooling**: Assumed ~300 W average draw, costing roughly $150‑$300 USD per year in electricity and cooling.
- **Hidden costs**: Includes admin time, occasional hardware failure downtime, and floor‑space considerations (see [[concepts/hidden-costs]]).
- **Utilization break‑even**: Becomes cost‑effective when sustained utilization exceeds roughly 50‑60 % of available hours (see [[concepts/utilization-break-even]]).
- **Hybrid role**: Serves as the baseline compute resource for nightly batch jobs, with occasional cloud bursting for spikes (see [[concepts/cost-analysis]] and hybrid compute strategy).
- **Metrics to monitor**: queue wait time, utilization level, and data transfer volume are the top three indicators for deciding when to burst to the cloud.

## Related Entities & Concepts
- Comparable cloud alternative: [[entities/cloud-compute]]
- Potential GPU option for the workstation: [[entities/gpu-instance]]

## Relevant Summary
- Detailed discussion of this workstation appears in [[summaries/session-13_2024-06-15]].