---
sources: ["summaries/session-03_2023-06-09.md"]
type: "Product"
description: "A short valve/manifold for equalizing differential sensor ports during zero checks."
---

# Equalization Valve / Manifold

**Type:** product

**Overview**
The equalization valve (or manifold) is a compact plumbing component used to momentarily expose both ports of a differential pressure sensor to the same ambient air pressure. By providing a common, low‑volume path that can be opened and closed on demand, it enables a quick, repeatable zero‑check without disconnecting tubing or introducing handling‑induced pressure spikes.

**Key Characteristics (from [[summaries/session-03_2023-06-09]])**
- **Configuration:** a small tee or manifold that joins the two sensor ports to a single equalization chamber, plus a controlled opening to ambient air.
- **Design goals:** short and rigid flow path, low‑leak fittings, minimal dead volume to reduce bias and pressure traps.
- **Operation:** open the valve to let both ports see the same ambient air for a few seconds, then close it to resume normal measurement.
- **Benefits:**
  - Provides a repeatable zero reference for [[entities/differential-pressure-sensor]]
  - Avoids the need to pop hoses on/off, reducing transient pressure disturbances.
  - Supports consistent documentation in the sensor drift workflow described in [[concepts/differential-zero-check]].

**Related Concepts**
- [[concepts/differential-zero-check]] – the procedure enabled by this valve.
- [[concepts/pressure-sensor-calibration]] – the broader calibration routine where the valve is used.
- [[concepts/sensor-drift-logging]] – logging the zero‑check results helps separate true sensor drift from environmental effects.

**Related Entities**
- [[entities/differential-pressure-sensor]] – the sensor type that directly benefits from the valve.
- [[entities/piezoresistive-absolute-pressure-sensor]] – other pressure sensors in the same lab setup.
- [[entities/data-acquisition-system]] – records the zero‑check readings captured via the valve.

**Practical Advice**
1. **Keep the equalization path short and stiff** to limit flex‑induced bias.
2. **Use fittings rated for low leakage** (e.g., metal‑to‑metal fittings) to prevent slow drifts during checks.
3. **Integrate the valve into the routine checklist** (daily/weekly/monthly) so zero checks are logged consistently.
4. **Document the valve state** (open/closed) and any ambient conditions in the CSV log schema to correlate with sensor drift trends.
