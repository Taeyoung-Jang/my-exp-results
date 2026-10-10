---
sources: ["summaries/session-03_2023-06-09.md"]
type: "Product"
description: "A piezoresistive absolute pressure sensor used for high‑altitude lab measurements."
---

## Piezoresistive Absolute Pressure Sensor

A **piezoresistive absolute pressure sensor** is a solid‑state transducer that converts pressure into an electrical resistance change, providing a direct measurement of absolute pressure relative to vacuum. In the context of high‑altitude laboratory work, these sensors are valued for their robustness and stability but require careful calibration because the operating altitude (e.g., 3,800 m) deviates significantly from the manufacturer’s reference conditions.

### Key Facts from [[summaries/session-03_2023-06-09]]
- **Calibration routine**: The document outlines a daily, weekly, and monthly checklist to ensure consistent performance. The sensor is calibrated against a **[[entities/reference-barometer]]** under stable ambient conditions.
- **Drift monitoring**: Offsets between the sensor reading and the reference are logged to separate true sensor drift from environmental effects, a practice described in [[concepts/sensor-drift-logging]].
- **Data capture**: An expanded CSV schema records fields such as `warmup_minutes`, `daq_channel`, `daq_scaling_version`, and `check_type` to contextualize each measurement.
- **Integration with DAQ**: The sensors are connected to a **[[entities/data-acquisition-system]]**, and scaling version information is tracked during each calibration.
- **Handling and storage**: Recommendations include keeping the sensors in a temperature‑stable environment and avoiding rapid pressure swings between runs.

### Related Concepts and Entities
- [[concepts/pressure-sensor-calibration]] – overall approach to establishing sensor accuracy.
- [[concepts/differential-zero-check]] – method for zeroing **[[entities/differential-pressure-sensor]]**; useful for comparative setups.
- [[entities/equalization-valve]] – hardware suggested for repeatable zero checks on differential sensors, which may be part of a mixed‑sensor system.

### Practical Use
When deploying these sensors at high altitude, follow the structured checklist to:
1. Warm‑up the sensor and DAQ for a defined period.
2. Perform a spot check against the reference barometer.
3. Log all relevant metadata using the provided CSV schema.
4. Review offset trends over weeks to decide if calibration intervals need shortening.

By adhering to this regimen, laboratories can maintain measurement fidelity despite the challenging environmental conditions.
