---
type: "Concept"
sources: ["summaries/session-06_2024-06-12.md"]
description: "Verifying external power sources and cables before board‑level diagnosis."
---

# External Power Verification

**Definition**: The process of confirming that the power supplied to a device from outside sources (wall outlet, USB‑C charger, battery pack, cables, adapters) is functional and not the cause of a failure.

---

## Why It Matters
In the diagnostic workflow described in [[summaries/session-06_2024-06-12]], the very first step is to rule out any external issue. A dead device often appears to have an internal fault when, in fact, the problem lies in a faulty outlet, broken cable, or depleted battery. Eliminating these possibilities saves time and prevents unnecessary invasive probing.

---

## Core Steps
1. **Visual Inspection**
   - Look for obvious damage to the power connector, frayed cables, or bent pins.
2. **Swap Known‑Good Components**
   - Use a different wall outlet, charger, or USB‑C cable that you know works with another device.
3. **Measure Input Voltage**
   - With a multimeter, check the voltage at the device’s input jack or USB‑C port. This aligns with the [[concepts/multimeter_power_checklist]] for confirming that power reaches the board.
4. **Check Battery Condition**
   - If the device has an internal Li‑ion cell, verify its voltage with a multimeter. A dead or severely depleted cell can prevent the device from powering up.
5. **Confirm Power Presence Before Opening**
   - Only proceed to internal inspection once you have verified that the external supply is delivering the expected voltage.

---

## Relationship to Other Concepts
- Serves as the entry point for the broader [[concepts/power_path_troubleshooting]] workflow.
- Complements the [[concepts/multimeter_power_checklist]] for voltage and continuity checks.
- If external power is confirmed, the next steps may involve [[concepts/bench_supply_short_detection]] or analyzing regulator behavior via [[concepts/buck_regulator_scope_signatures]].
- When visual clues are insufficient, a detailed board photograph can aid the process, linking to [[concepts/photo_based_board_analysis]].

---

## Practical Tips
- Always test with the device unplugged from any other power source to avoid confusing readings.
- Use a multimeter set to DC voltage; avoid auto‑range if you know the expected level (e.g., 5 V for USB‑C).
- If the measured voltage is significantly lower than expected, the fault is likely in the cable or connector rather than the device itself.

---

*This concept is derived from the diagnostic discussion in [[summaries/session-06_2024-06-12]].*