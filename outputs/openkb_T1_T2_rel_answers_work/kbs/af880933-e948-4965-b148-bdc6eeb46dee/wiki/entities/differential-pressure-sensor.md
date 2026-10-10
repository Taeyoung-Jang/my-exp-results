---
sources: ["summaries/session-03_2023-06-09.md"]
type: "Product"
description: "A differential pressure sensor used in high‑altitude lab calibration routines."
---

# Differential Pressure Sensor

**Type:** product

The differential pressure sensor referenced in the lab workflow is a piezoresistive device that measures pressure differences between two ports. It is typically integrated with a **data‑acquisition system** (DAQ) for real‑time monitoring and logging.

## Key Facts from Session 3 (2023‑06‑09)
- **Application context:** Used in a high‑altitude laboratory (≈ 3,800 m) where ambient pressure variations can influence sensor drift.
- **Calibration routine:** Subject to the same daily, weekly, and monthly checklist outlined for pressure sensor calibration, with emphasis on consistent ambient conditions and thermal warm‑up.
- **Logging requirements:** Calibration logs should capture fields such as `daq_channel`, `daq_scaling_version`, `warmup_minutes`, and `check_type` to trace sensor performance over time. See the expanded CSV schema in the session summary.
- **Zero‑check method:** A quick field zero check is performed by equalizing both ports to the same ambient air using an **equalization valve** or manifold, avoiding disconnections that could introduce pressure pulses.
- **Hardware recommendation:** A short, rigid tee or manifold that connects both sensor ports to a common chamber with a controlled opening to ambient air minimizes bias and leakage, providing repeatable zero‑check results.

## Related Concepts
- [[concepts/pressure-sensor-calibration]]
- [[concepts/sensor-drift-logging]]
- [[concepts/differential-zero-check]]

## Related Entities
- [[entities/data-acquisition-system]]
- [[entities/equalization-valve]]
- [[entities/piezoresistive-absolute-pressure-sensor]] (often used alongside differential sensors)
- [[entities/reference-barometer]] (used as the reference standard during calibration)

## Source Summary
For a concise overview of the checklist and log schema that reference this sensor, see the session summary: [[summaries/session-03_2023-06-09]].