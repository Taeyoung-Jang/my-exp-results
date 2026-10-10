---
type: "Concept"
sources: ["summaries/session-06_2024-06-12.md"]
description: "Using a current‑limited bench supply to locate shorts on a dead board."
---

# Bench Supply Short Detection

**Definition**: A diagnostic technique that applies a reduced‑voltage, current‑limited bench power supply to a suspect power rail in order to identify the location of a short circuit without damaging components.

---

## Why Use a Bench Supply?
- When a device shows **no power** and multimeter checks indicate a possible short, directly powering the board can cause overheating or further damage.
- A bench supply lets you **control voltage** and **limit current**, providing a safe way to feed the rail and observe where excess current is drawn.

## Typical Workflow
1. **Set Up**
   - Choose a voltage **slightly lower** than the rail’s normal operating voltage (e.g., 4.5 V for a 5 V rail).
   - Set the **current limit** to a low value (often 100 mA to 300 mA) to prevent runaway heating.
2. **Connect** the supply to the rail’s input pin or test point while the rest of the board remains unpowered.
3. **Observe**:
   - If the current stays well below the limit and the voltage remains stable, the rail is likely free of a hard short.
   - If the current quickly reaches the limit and the supply voltage drops, the excess current is being absorbed somewhere downstream.
4. **Locate the Hot Spot**
   - Carefully **touch** a temperature‑sensitive probe or use a fingertip (quickly) to feel for the warmest component or trace.
   - The area that heats up most is a strong indicator of the short’s location.
5. **Confirm**
   - Once a suspect component or trace is identified, you can perform a more focused continuity or resistance check (see [[concepts/multimeter_power_checklist]]) to verify the fault.

## Safety Tips
- **Discharge** any capacitors on the board before attaching the supply.
- Keep the current limit **low** initially; increase only if the board tolerates it.
- Do **not** keep the supply on for more than a few seconds; prolonged heating can damage the board.
- Wear **protective eyewear** and have a **fire‑extinguishing** method nearby.

## Relationship to Other Concepts
- This technique is often the **next step** after performing an external verification of power sources [[concepts/external_power_verification]].
- It complements the **multimeter checklist** for checking resistance and diode drops when the board is unpowered [[concepts/multimeter_power_checklist]].
- After locating a short, you may need to decide whether the fault is in a **buck regulator**; the corresponding scope signatures are described in [[concepts/buck_regulator_scope_signatures]].
- The overall diagnostic flow fits within the broader **power‑path troubleshooting** methodology [[concepts/power_path_troubleshooting]].
- Visual inspection of the board, possibly aided by photos, is covered in [[concepts/photo_based_board_analysis]].

---

**Reference**: This concept is derived from the discussion in [[summaries/session-06_2024-06-12]], where a practical, safety‑first workflow for a dead handheld device was outlined.
