---
type: "Concept"
sources: ["summaries/session-40_2024-12-10.md", "summaries/session-03_2023-06-09.md"]
description: "Method for quickly verifying zero offset of differential pressure sensors in the field."
---

# Differential Sensor Zero‑Check

**Definition**: A rapid, low‑error procedure to verify that a differential pressure sensor reads zero when both its input ports are exposed to the same pressure, typically ambient air, without disconnecting tubing.

---

## Why it matters
At high altitude labs (e.g., 3,800 m) differential sensors are especially prone to drift and handling‑induced bias. A reliable zero‑check helps distinguish true sensor drift from transient errors introduced during hose or port manipulation, supporting accurate [[concepts/pressure-sensor-calibration]] and consistent [[concepts/sensor-drift-logging]].

---

## Core steps (field‑ready)
1. **Equalize ports** – Use an equalization valve or a short tee/manifold that simultaneously connects both sensor ports to a common ambient air source.  The valve should be opened briefly so that both sides see the same pressure.
2. **Stabilize** – Allow a few seconds for any pressure transients to settle; the shared path should be short and rigid to minimise lag.
3. **Read zero** – Record the sensor output.  The reading should be near the manufacturer‑specified zero (typically within a few Pa).
4. **Close valve** – Return the sensor to its normal measurement lines by closing the equalization valve.
5. **Document** – Log the timestamp, sensor ID, check_type = "daily spot check" (or whatever routine applies), ambient temperature, and any handling notes.

---

## Hardware recommendation
A practical implementation is a compact **equalization valve** (see [[entities/equalization-valve]]) that links the two ports via a low‑volume, low‑leak manifold.  Keep the equalization path short and use fittings rated for minimal leakage to reduce bias.  When the valve is closed, the sensor resumes its regular measurement configuration without needing to disconnect tubing, thus avoiding hose‑handling errors.

---

## Integration with logging
The zero‑check results should be captured in the expanded CSV schema described in [[summaries/session-03_2023-06-09]], using fields such as:
- `check_type` (e.g., "daily" or "weekly")
- `warmup_minutes`
- `daq_channel` and `daq_scaling_version` (if applicable)
- `ambient_temp_C` and `ambient_pressure_hPa`
- `handling_notes` (e.g., "valve opened 5 s, settled 3 s")

These entries enable trend analysis to separate true sensor drift from occasional handling‑induced offsets.

---

## Related concepts
- [[concepts/differential-zero-check]] (this page)
- [[concepts/pressure-sensor-calibration]]
- [[concepts/sensor-drift-logging]]

---

*Referenced source*: [[summaries/session-03_2023-06-09]]

See also: [[summaries/session-40_2024-12-10]]