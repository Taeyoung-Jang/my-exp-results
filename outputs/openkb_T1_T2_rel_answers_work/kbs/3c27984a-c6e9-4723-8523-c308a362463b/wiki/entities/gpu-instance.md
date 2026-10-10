---
sources: ["summaries/session-13_2024-06-15.md"]
type: "Product"
description: "On‑demand cloud GPU compute resource referenced for simulation bursts"
---

## GPU Instance

A **GPU Instance** is a cloud‑based compute offering that provides one or more graphics processing units (GPUs) for high‑performance workloads such as simulation, rendering, or machine‑learning tasks. In the context of the *session‑13_2024‑06‑15* discussion, a GPU Instance represents the cloud alternative to a local workstation when bursting compute for occasional spikes.

### Key points from the document
- Used as the cloud counterpart to a **local workstation** for running heavy simulations.
- Cost is evaluated per‑hour, combined with storage and data‑egress fees to estimate a marginal job cost.
- Recommended for burst scenarios where local utilization exceeds the break‑even point (≈50‑60% sustained usage) or queue wait time passes a defined threshold.
- Incorporates hidden costs such as specialized hardware premiums and licensing that affect overall cloud cost.

### Related concepts and entities
- [[concepts/cost-analysis]] – framework for comparing total cost of ownership.
- [[concepts/hidden-costs]] – includes storage, egress, and premium hardware fees.
- [[concepts/utilization-break-even]] – utilization level where GPU Instance becomes cost‑effective.
- [[entities/local-workstation]] – the on‑premise hardware alternative.
- [[summaries/session-13_2024-06-15]] – source document where the GPU Instance is discussed.