---
type: "Concept"
sources: ["summaries/session-39_2025-06-15.md", "summaries/session-13_2024-06-15.md"]
description: "Unexpected expenses that affect total cost of local or cloud compute."
---

# Hidden Costs

**Hidden Costs** are the indirect or easily overlooked expenses that influence the true economic comparison between [[entities/local-workstation]] and [[entities/cloud-compute]] for compute‑heavy simulations.  The concept is discussed in detail in [[summaries/session-13_2024-06-15]].

## Typical hidden costs for local hardware
- **Power and cooling** – electricity for a several‑hundred‑watt machine and the associated cooling infrastructure, often estimated at a few hundred dollars per year.
- **Floor space, noise, and environmental** – physical space, ventilation, and acoustic considerations can add operational overhead.
- **Hardware replacement / warranty extensions** – part wear, upgrades, and optional service contracts.
- **Administrative time** – regular updates, driver fixes, monitoring, and troubleshooting (often approximated as an hour per week of staff time).
- **Downtime** – lost productivity from component failures or maintenance windows.

## Typical hidden costs for cloud resources
- **Long‑term storage fees** – persistent block or object storage charges that accrue even when the instance is idle.
- **Data egress charges** – per‑GB fees for moving results or intermediate data out of the cloud, which can dominate the bill for large outputs.
- **Specialized hardware premiums** – higher hourly rates for GPU or high‑performance instances compared to standard CPUs.
- **Licensing models** – software licenses that vary in cost depending on whether they run on‑premise or in the cloud.

## Relationship to other concepts
- The identification of hidden costs is a key step in performing a thorough [[concepts/cost-analysis]].
- Understanding these expenses helps define the [[concepts/utilization-break-even]] point, where the total cost of ownership of a [[entities/local-workstation]] matches the pay‑as‑you‑go expense of [[entities/cloud-compute]].

## Practical use
When evaluating a compute strategy, list both the obvious line items (hardware purchase price, instance hourly rate) and the hidden costs above.  Subtracting these from the projected budget yields a more realistic comparison and informs decisions such as whether to adopt a hybrid approach or implement a bursting rule.


See also: [[summaries/session-39_2025-06-15]]