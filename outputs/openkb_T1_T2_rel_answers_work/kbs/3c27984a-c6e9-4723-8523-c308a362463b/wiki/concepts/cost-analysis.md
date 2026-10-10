---
type: "Concept"
sources: ["summaries/session-39_2025-06-15.md", "summaries/session-13_2024-06-15.md"]
description: "Framework for comparing total cost of local vs cloud compute resources."
---

# Cost Analysis

Cost analysis is the systematic comparison of the total expenses associated with running compute‑heavy simulations on a **local workstation** versus using **cloud compute** resources. It combines both direct and indirect costs to produce an effective $/hour figure for each option, enabling a break‑even assessment.

## Core Elements

1. **Annualized Local Cost**
   - Capital expense amortized over the hardware lifespan (e.g., a $10k [[entities/local-workstation]] spread over 3 years).
   - Power consumption and cooling (electricity cost per kWh).
   - Maintenance, admin time, and expected downtime.
   - Resulting in an *effective hourly cost* that depends on actual utilization.

2. **Cloud Per‑Hour Cost**
   - On‑demand hourly rate for a comparable [[entities/gpu-instance]] or CPU instance from a cloud provider.
   - Storage fees for input data and temporary results.
   - Data egress charges when pulling results back to the local environment.

3. **Break‑Even Utilization**
   - The utilization level at which the local effective hourly cost equals the cloud hourly cost.  In the source discussion, a sustained utilization of roughly **50‑60 %** is identified as the threshold where local hardware starts to be cheaper.  This relationship is captured in the [[concepts/utilization-break-even]] concept.

4. **Hidden Costs**
   - Expenses that are easy to overlook but can shift the balance: electricity, cooling, floor space, hardware replacement, admin overhead for local; storage, egress, specialized hardware premiums, and licensing for cloud.  See the [[concepts/hidden-costs]] concept for a deeper dive.

## Applying the Framework

- **Step 1:** Compute the annualized local cost using the components above.
- **Step 2:** Estimate the cloud cost per job: `instance_rate × runtime + storage_cost + egress_cost`.
- **Step 3:** Compare the two using the utilization break‑even point.  If expected utilization is above the break‑even, local is preferred; otherwise, cloud (or a hybrid model) is more economical.
- **Step 4:** Re‑evaluate periodically as hardware ages, electricity rates change, or cloud pricing evolves.

## Example from Session 13

The discussion in [[summaries/session-13_2024-06-15]] walks through a concrete example: a $10k workstation amortized to ~$3.3k per year, plus ~$300 / yr for power and cooling, and several hundred dollars for admin time, yielding an approximate **$1 / hour** effective cost at 50 % utilization.  Cloud GPU instances were quoted at **$5‑$10 / hour**, plus storage and egress, illustrating the break‑even calculation.

## Related Concepts

- [[concepts/hidden-costs]]
- [[concepts/utilization-break-even]]

---
*This concept page synthesizes the cost‑analysis approach presented in the source summary and provides a reusable framework for evaluating compute‑resource decisions.*

See also: [[summaries/session-39_2025-06-15]]