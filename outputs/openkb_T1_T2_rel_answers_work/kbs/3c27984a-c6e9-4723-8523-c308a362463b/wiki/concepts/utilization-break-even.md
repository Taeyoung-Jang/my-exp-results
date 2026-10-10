---
type: "Concept"
sources: ["summaries/session-39_2025-06-15.md", "summaries/session-13_2024-06-15.md"]
description: "Utilization level where local hardware cost equals cloud compute cost."
---

# Utilization Break‑Even

The **Utilization Break‑Even** concept defines the sustained usage percentage at which the total cost of owning and operating a local machine matches the pay‑as‑you‑go cost of equivalent cloud resources. Below this point, cloud compute is generally cheaper; above it, a local workstation becomes more cost‑effective.

## Core Idea
- Compute the **effective hourly cost** of a local setup by amortizing the purchase price, adding power, cooling, admin time, and expected downtime.
- Compute the **per‑hour cloud cost** for an equivalent instance (including instance price, temporary storage, and data egress).
- The break‑even utilization is the fraction of time the local machine must be busy for the two costs to intersect.

## Numerical Illustration from [[summaries/session-13_2024-06-15]]
- A $10 k workstation spread over 3 years → ≈ $3,300 / year.
- Power & cooling ≈ $300 / year; admin & downtime ≈ $400 / year.
- **Total local cost** ≈ $4,000 / year → about **$1 / hour** if used ~4,400 h (≈ 50 % of yearly hours).
- Cloud GPU instance rates range from $2 – $10 / hour plus storage/egress.
- Resulting break‑even utilization falls around **50‑60 % sustained usage**.

## Practical Usage
1. **Estimate local all‑in cost** (hardware amortization + hidden costs).
2. **Identify comparable cloud instance** (e.g., a [[entities/gpu-instance]] on [[entities/cloud-compute]]).
3. **Calculate hourly rates** and solve for utilization where:
   ```
   local_hourly_cost / utilization = cloud_hourly_rate
   ```
4. Use this threshold to decide when to burst to the cloud.

## Related Concepts
- [[concepts/cost-analysis]] – overall financial comparison methods.
- [[concepts/hidden-costs]] – factors like electricity, cooling, admin time, and egress that affect both sides of the equation.

## Decision Guidance
- **If utilization > break‑even** → prefer local hardware for cost savings.
- **If utilization < break‑even** → cloud offers cheaper pay‑per‑use pricing and flexibility.
- For mixed workloads (e.g., nightly batches with occasional spikes), a **hybrid approach** uses the local machine as baseline and triggers cloud bursting when utilization crosses the break‑even point.


See also: [[summaries/session-39_2025-06-15]]