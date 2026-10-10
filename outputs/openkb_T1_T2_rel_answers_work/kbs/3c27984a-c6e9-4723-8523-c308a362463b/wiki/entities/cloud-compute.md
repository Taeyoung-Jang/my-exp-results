---
sources: ["summaries/session-13_2024-06-15.md"]
type: "Product"
description: "On‑demand cloud‑based compute resources for heavy simulations."
---

# Cloud Compute

Cloud Compute refers to on‑demand, remotely hosted compute resources that can be provisioned as needed for workloads such as compute‑heavy simulations. In the context of the session‑13 discussion, it is presented as an alternative to owning a [[entities/local-workstation]] and is evaluated using several analytical lenses.

## Key Points from the Session

- **Cost model**: Users pay per‑hour for instances (including GPU options), plus storage and data egress fees. The document recommends a [[concepts/cost-analysis]] that aggregates instance rates, temporary storage, and egress to estimate a marginal cost per job.
- **Hidden costs**: While eliminating upfront hardware spend, Cloud Compute incurs hidden expenses like long‑term storage, egress charges, specialized hardware premiums, and potential licensing differences – captured under [[concepts/hidden-costs]].
- **Break‑even utilization**: The analysis suggests a break‑even point around 50‑60% sustained utilization; above this, a [[entities/local-workstation]] may be cheaper, while bursty workloads benefit from Cloud Compute, referencing [[concepts/utilization-break-even]].
- **Hybrid strategy**: For workloads that run nightly batches with occasional spikes, a hybrid model is advised – keep a baseline local box and burst to Cloud Compute when queue delays or utilization exceed set thresholds.
- **Relevant resources**: Typical Cloud Compute offerings may include [[entities/gpu-instance]] types when GPU acceleration is needed.

## Relation to the Document

The detailed comparison, cost framework, and bursting rule are discussed in [[summaries/session-13_2024-06-15]]. This entity page synthesizes those points to describe the role and considerations of Cloud Compute in a mixed on‑premise/cloud workflow.