---
type: "Concept"
sources: ["summaries/session-34_2025-10-08.md"]
description: "Framework for scheduling multiple short trips efficiently under constraints."
---

# Errand Planning

**Definition** – A systematic approach to sequencing and timing short, often disparate, trips (e.g., grocery pick‑up, pharmacy, returns) so that total travel time, walking distance, and wait time are minimized while respecting personal constraints such as mobility limits or strict time windows.

## Core Elements
1. **Timing Window** – Identify a start time that aligns with low‑traffic periods at each stop. In the example from [[summaries/session-34_2025-10-08]], a Saturday 8:45 a.m. departure captures quiet store openings.
2. **Stop Sequencing** – Order stops to reduce back‑tracking. The plan moves linearly: Target → CVS → Kohl’s → Old Navy.
3. **Curbside & Drive‑Through Utilization** – Leverage services that keep you in the car to limit walking. This ties directly to [[concepts/curbside-pickup]].
4. **Parking Strategy** – Choose parking spots that serve multiple stops (e.g., front‑row spot at the Kohl’s entrance) to avoid re‑parking. See [[concepts/parking-strategy]].
5. **Backup Procedures** – Define thresholds for when to abandon a delayed service (e.g., cancel Target check‑in after a 5‑minute wait) and an alternative sequence.

## Practical Tips from the Source
- **Pre‑Check‑In** – Initiate the Target Drive‑Up check‑in a few minutes before arrival (8:50 a.m.) to have the order staged.
- **Entity‑Specific Actions**
  - [[entities/target]]: Use Drive‑Up and cancel if delayed.
  - [[entities/cvs]]: Call ahead for drive‑thru readiness.
  - [[entities/kohls]]: Amazon return via QR code, no box needed.
  - [[entities/old-navy]]: In‑store return; ask staff for side register if line builds.
- **Time Buffer** – Allocate ~10 minutes per stop plus a 5‑minute buffer for unexpected delays, keeping the total under two hours.

## Benefits
- **Mobility‑Friendly** – Reduces standing and walking, crucial for users in a walking boot.
- **Time‑Efficient** – Keeps the entire errand run under a predefined duration.
- **Stress Reduction** – Pre‑planning, check‑ins, and backup options minimize on‑the‑spot decision‑making.

---
*Related concepts*: [[concepts/curbside-pickup]], [[concepts/parking-strategy]]
