---
type: "Concept"
sources: ["summaries/session-40_2024-12-10.md", "summaries/session-03_2023-06-09.md"]
description: "Systematic recording of sensor offsets and environment to track pressure sensor drift."
---

# Sensor Drift Logging

**Definition**: Sensor drift logging is the systematic capture of measurement offsets and contextual metadata for pressure sensors over time, enabling analysts to distinguish true sensor degradation from environmental influences.

## Why It Matters
- In high‑altitude labs, ambient pressure and temperature variations can masquerade as sensor drift. By logging both the sensor reading and the surrounding conditions, teams can identify whether changes are **environmental** or **intrinsic** to the sensor.
- Consistent drift logs support **trend analysis**, prompting earlier recalibration or hardware replacement before performance degrades.

## Core Log Fields (as suggested in [[summaries/session-03_2023-06-09]])
| Field | Purpose |
|---|---|
| `timestamp` | Exact date‑time of the measurement. |
| `sensor_id` | Identifier linking to a specific [[entities/piezoresistive-absolute-pressure-sensor]] or [[entities/differential-pressure-sensor]]. |
| `sensor_type` | Distinguishes absolute vs. differential devices. |
| `daq_channel` | Tracks which input on the [[entities/data-acquisition-system]] was used. |
| `daq_scaling_version` | Records the firmware/scale version applied during the reading. |
| `warmup_minutes` | Time the sensor was allowed to thermally stabilize before measurement. |
| `check_type` | Indicates whether the entry is from a **daily spot check**, **weekly verification**, or **monthly full calibration**. |
| `raw_reading` | The sensor’s output value. |
| `reference_reading` | Value from the calibrated [[entities/reference-barometer]]. |
| `offset` | Calculated difference (raw – reference). |
| `ambient_temp_C` | Ambient temperature, helps isolate temperature‑induced drift. |
| `ambient_pressure_hPa` | Ambient pressure, crucial for altitude‑sensitive sensors. |
| `storage_notes` | Observations about storage conditions between runs. |
| `handling_notes` | Any handling or setup remarks that could affect readings. |

## How It Supports [[concepts/pressure-sensor-calibration]]
- **Trend‑Based Interval Adjustment**: If logged offsets show a steady trend, calibration frequency can be increased before the next scheduled full calibration.
- **Environmental Correlation**: By correlating offsets with `ambient_temp_C` and `ambient_pressure_hPa`, users can decide whether to apply environmental compensation or to focus on sensor replacement.
- **Audit Trail**: Detailed logs provide traceability for quality‑control audits and help justify equipment maintenance decisions.

## Relationship to [[concepts/differential-zero-check]]
- For differential sensors, regular zero‑check results should also be entered into the drift log using the same schema, with `check_type` set to *daily* or *weekly*. This ensures zero‑point stability is tracked alongside absolute sensor drift.

## Implementation Tips
1. **Automate Capture**: Integrate the CSV schema directly with the [[entities/data-acquisition-system]] software to auto‑populate fields where possible.
2. **Central Repository**: Store logs in a version‑controlled location (e.g., a shared drive or database) to enable historical querying.
3. **Visualization**: Plot `offset` versus time, overlaying temperature and pressure trends to quickly spot correlation patterns.
4. **Review Cycle**: Schedule a monthly review of the log to assess drift rates and decide on any procedural changes.

---
*Concept page created to synthesize guidance from [[summaries/session-03_2023-06-09]] and support robust pressure sensor maintenance.*

See also: [[summaries/session-40_2024-12-10]]