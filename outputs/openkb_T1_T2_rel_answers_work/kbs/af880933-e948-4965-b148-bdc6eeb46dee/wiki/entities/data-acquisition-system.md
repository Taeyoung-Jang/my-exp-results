---
sources: ["summaries/session-03_2023-06-09.md"]
type: "Product"
description: "A product that interfaces with pressure sensors to acquire and scale measurement data."
---

# Data Acquisition System (DAQ)

A **Data Acquisition System (DAQ)** is the hardware and software platform used to collect, digitize, and scale signals from laboratory pressure sensors. In the context of the high‑altitude lab described in session 03 2022 06 09, the DAQ connects to both [[entities/piezoresistive-absolute-pressure-sensor]] and [[entities/differential-pressure-sensor]] units, providing channel‑specific scaling that is tracked during calibration routines.

## Key Facts from Session 3 (2023‑06‑09)
- **Sensor Integration**: The DAQ handles raw readings from piezoresistive absolute and differential pressure sensors, converting them to digital values for analysis.
- **Channel Identification**: Each sensor is assigned a specific DAQ channel, recorded in the CSV log schema under the `daq_channel` field.
- **Scaling Version**: The DAQ’s scaling firmware or configuration version (`daq_scaling_version`) is logged to ensure traceability of any changes that could affect sensor output.
- **Calibration Workflow**: During daily, weekly, and monthly checks, the DAQ’s scaling is verified as part of the [[concepts/pressure-sensor-calibration]] process. Offsets between raw sensor readings and the [[entities/reference-barometer]] are calculated and stored.
- **Drift Monitoring**: Offsets captured by the DAQ are used in [[concepts/sensor-drift-logging]] to distinguish true sensor drift from environmental effects such as temperature or altitude variations.
- **Differential Zero Check**: For differential sensors, the DAQ works with an [[entities/equalization-valve]] to perform a quick zero‑check, following the procedure outlined in [[concepts/differential-zero-check]].

## Related Concepts and Entities
- [[concepts/pressure-sensor-calibration]] – systematic approach to maintaining sensor accuracy.
- [[concepts/sensor-drift-logging]] – logging strategy for tracking sensor performance over time.
- [[concepts/differential-zero-check]] – method for verifying zero offset in differential pressure sensors.
- [[entities/equalization-valve]] – hardware used with the DAQ for repeatable zero checks.
- [[entities/reference-barometer]] – reference instrument against which DAQ readings are compared.

## Documentation Reference
Further details on the DAQ’s role in the calibration checklist and log schema can be found in the session summary: [[summaries/session-03_2023-06-09]].