---
type: "Concept"
sources: ["summaries/session-40_2024-12-10.md", "summaries/session-03_2023-06-09.md"]
description: "Standardized procedures for calibrating pressure sensors in high‑altitude labs."
---

# Pressure Sensor Calibration

**Definition**: A systematic approach to verify and adjust the output of pressure sensors—especially piezoresistive absolute and differential types—so that readings remain accurate under varying environmental conditions such as high altitude.

## Overview
Calibration is critical in environments like a 3,800 m lab where ambient pressure and temperature differ markedly from factory settings. The goal is to create repeatable, traceable measurements by following consistent routines and logging the results for trend analysis.

## Routine Checklist (Daily / Weekly / Monthly)
- **Daily**: Warm‑up sensors and the [[entities/data-acquisition-system]] to a stable temperature, compare each sensor to the [[entities/reference-barometer]], record raw and reference values, calculate the offset, and note any ambient swings or handling issues.
- **Weekly**: Repeat the daily steps, verify DAQ channel scaling and version, inspect cables and ports, and log offsets under the most stable conditions.
- **Monthly**: Perform a full calibration under controlled ambient conditions, document any adjustments, review month‑long offset trends, and confirm storage stability.

These steps embody the [[concepts/sensor-drift-logging]] practice by capturing consistent data points over time.

## Expanded CSV Log Schema
A recommended schema to capture all relevant variables:
```
timestamp, sensor_id, sensor_type, daq_channel, daq_scaling_version,
warmup_minutes, check_type, raw_reading, reference_reading, offset,
ambient_temp_C, ambient_pressure_hPa, storage_notes, handling_notes
```
- **check_type** distinguishes daily spot checks, weekly verification, and monthly full calibrations.
- Including **warmup_minutes** and **daq_scaling_version** improves traceability of each measurement.

## Differential Sensor Zero Check
For [[entities/differential-pressure-sensor]] units, a quick and repeatable zero‑check involves briefly equalizing both ports to the same ambient air using an [[entities/equalization-valve]] or tee manifold. This method avoids hose disconnections and minimizes pressure pulses, aligning with the [[concepts/differential-zero-check]] approach.

## Hardware Recommendation: Equalization Valve/Manifold
- Install a short, rigid tee that joins both sensor ports to a common chamber.
- Provide a controlled valve opening to ambient air for the zero‑check.
- Use low‑leak fittings to prevent bias and ensure repeatability.
- When closed, the measurement lines revert to normal operation.

## Benefits
- **Consistency**: Same ambient conditions and warm‑up times reduce variability.
- **Traceability**: Detailed logs enable separation of true sensor drift from environmental effects.
- **Efficiency**: Daily spot checks catch large deviations early; weekly and monthly routines manage long‑term stability.

## Related Concepts
- [[concepts/differential-zero-check]]
- [[concepts/sensor-drift-logging]]

## Source
- Detailed checklist, log schema, and hardware advice are derived from [[summaries/session-03_2023-06-09]].

See also: [[summaries/session-40_2024-12-10]]