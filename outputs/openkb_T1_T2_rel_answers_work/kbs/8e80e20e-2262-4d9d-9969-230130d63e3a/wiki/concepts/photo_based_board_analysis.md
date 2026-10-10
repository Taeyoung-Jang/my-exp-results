---
type: "Concept"
sources: ["summaries/session-06_2024-06-12.md"]
description: "Using board photos to map power stages and guide troubleshooting."
---

# Photo‑Based Board Analysis

**Definition** – A visual‑inspection workflow that relies on photographs of a circuit board (wide‑angle and macro shots) to identify the power‑path topology, locate potential failure points, and prioritize diagnostic steps.

---

## Why Use Photographs?
- Provides a **non‑invasive** first look before any probing.
- Allows remote assistance: the analyst can recognize component types, IC markings, inductors, and layout patterns.
- Helps spot **obvious physical defects** (cracked solder joints, burnt parts, missing components) that may not be evident with a multimeter alone.

## Typical Photo Set
1. **Wide shot of the input area** – Shows the USB‑C connector, any barrel jack, and the immediate surrounding traces.
2. **Macro shots of power‑related ICs** – Capture part numbers, pin‑1 orientation, and nearby passives.
3. **Close‑ups of inductors and large MOSFETs** – Reveal the likely buck/boost stages.
4. **Bottom‑side view (if accessible)** – Exposes hidden vias, ground planes, and additional components.

## Visual Cues to Identify Power Stages
| Visual Feature | Likely Function |
|---|---|
| Thick copper traces from the connector | **Input / protection** (fuse, reverse‑polarity diode/MOSFET) |
| Small SMD diode or TVS near the connector | **Transient protection** |
| Large inductor with adjacent diode or MOSFET | **Switching regulator (buck/boost)** |
| Small 3‑pin IC with “LDO” or “REG” marking | **Low‑dropout regulator** |
| Battery‑management IC (often QFN with multiple pins) | **Charging / power‑path controller** |

## Workflow Integration
1. **Collect photos** as described above.
2. **Map the power‑path** using the visual cues, creating a block diagram of stages.
3. Cross‑reference the identified stages with the diagnostic checklist in [[concepts/multimeter_power_checklist]] to decide which rails to probe first.
4. If a stage appears suspect (e.g., missing inductor or burnt component), use the **bench‑supply short detection** method from [[concepts/bench_supply_short_detection]] to safely test continuity.
5. When a regulator stage is reachable, verify its switching behavior with a scope, consulting [[concepts/buck_regulator_scope_signatures]] for expected waveforms.
6. Throughout, keep the **external power verification** steps from [[concepts/external_power_verification]] in mind to rule out cable or adapter issues before board‑level work.

## Example from Session 06 (2024‑06‑12)
In the referenced conversation, the user was asked to provide a wide‑angle shot of the USB‑C area and macro images of the IC markings.  The assistant explained that these images would allow the analyst to:
- Identify the **input protection** block.
- Locate the **charging controller** and **buck regulators**.
- Prioritize checking the first stage where power may be lost, following the **power‑path troubleshooting** approach described in [[concepts/power_path_troubleshooting]].

## Benefits
- Reduces unnecessary probing, protecting delicate components.
- Enables remote collaboration; experts can guide the user without being on‑site.
- Provides a documented visual record for future reference or warranty claims.

---

**Related concepts**: [[concepts/external_power_verification]], [[concepts/multimeter_power_checklist]], [[concepts/bench_supply_short_detection]], [[concepts/buck_regulator_scope_signatures]], [[concepts/power_path_troubleshooting]]

**Source summary**: [[summaries/session-06_2024-06-12]]