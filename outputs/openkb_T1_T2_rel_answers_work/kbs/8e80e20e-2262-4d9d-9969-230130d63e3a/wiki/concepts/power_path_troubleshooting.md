---
type: "Concept"
sources: ["summaries/session-06_2024-06-12.md"]
description: "Systematic method for diagnosing power‑delivery failures in consumer electronics."
---

# Power Path Troubleshooting

**Definition**: A structured workflow for locating and diagnosing failures along the electrical power delivery chain of a device, from external source to internal rails.

---

## Overview
Power path troubleshooting focuses on **sequential verification** of each functional block that conveys power from the connector to the end‑use rails. By treating the power delivery network as a *tree* of stages, you can isolate the point where voltage stops propagating.

The approach is particularly useful for handheld or small consumer devices that:
- Accept power via USB‑C or a barrel jack
- Contain a single‑cell Li‑ion battery
- Use a combination of protection circuitry, charging controller, buck converters and LDOs

## Typical Stages in the Power Tree
1. **External Power Verification** – Ensure the outlet, cable, adapter, and battery are functional before probing the board.  
   *Related concept*: [[concepts/external_power_verification]]
2. **Input Connector & Initial Traces** – Locate the USB‑C pins or barrel‑jack leads, check for continuity to the first large copper trace.
3. **Protection Circuitry** – Fuse, reverse‑polarity diode or MOSFET, often the thickest traces radiating from the connector.
4. **Charging / Power‑Path Controller** – Dedicated IC that manages battery charging and distributes power to downstream rails.
5. **Primary Regulators** – Buck or boost converters that generate the main system voltage(s).
6. **Secondary Rails** – LDOs or additional buck stages that supply low‑noise or specific voltage domains.

At each stage you **measure** (voltage, continuity) and **observe** (heat, LED activity, audible cues) before moving to the next.

---

## Core Checklist (derived from [[summaries/session-06_2024-06-12]])
| Step | Action | Expected Observation |
|------|--------|----------------------|
| 1 | Verify external power source works (swap cable, use known‑good charger). | Device powers on or at least shows LED activity. |
| 2 | With the board *unpowered*, use a multimeter in **diode/ohms** mode to probe the input line. Look for a low resistance to ground (possible short) or a normal one‑direction drop (healthy protection). | Near‑zero resistance → short; normal drop → path likely intact. |
| 3 | Power the board and measure voltage at the **input connector**. | Nominal USB‑C voltage (~5 V) or barrel‑jack voltage. |
| 4 | Measure after the **protection block** (fuse/diode). | Same as step 3 if protection is intact; lower or zero if fused/open. |
| 5 | Probe the **charging controller** pins (input and output rails). | Input present, output present if controller is alive. |
| 6 | Test **primary buck/regulator** input and output. Use a scope to check for switching activity. | Switching pulses → regulator enabled; flat line → regulator disabled. |
| 7 | Verify **secondary rails** (LDO outputs). | Expected rail voltages (e.g., 3.3 V, 1.8 V). |

If a stage fails to show the expected voltage, you have isolated the fault to that block.

---

## Diagnostic Tools
- **Multimeter** – Voltage, continuity, diode/ohms modes.  
  *Related concept*: [[concepts/multimeter_power_checklist]]
- **Current‑limited bench supply** – Inject a safe voltage with a low current limit to locate shorts.  
  *Related concept*: [[concepts/bench_supply_short_detection]]
- **Oscilloscope** – Observe switching waveforms to differentiate an overloaded buck from a disabled regulator.  
  *Related concept*: [[concepts/buck_regulator_scope_signatures]]
- **Visual inspection & photos** – Use macro images to map component locations and identify obvious damage.  
  *Related concept*: [[concepts/photo_based_board_analysis]]

---

## Practical Example (from the session)
The user’s handheld device was *completely dead* (no LED, no draw). Following the power‑path workflow:
1. **External check** – Swapped cable, still dead.
2. **Diode/Ohms test** – Input line showed a near‑zero resistance both directions → likely short downstream.
3. **Bench‑supply test** – Applied 5 V with a 200 mA limit; the board warmed at a specific copper area, pinpointing the short location.
4. **Scope check** – After removing the short, the buck regulator’s input had voltage but no switching activity, indicating the regulator was not being enabled.

This systematic isolation saved time and avoided unnecessary component replacement.

---

## When to Stop and Escalate
- If a short is located on a dense area (e.g., under an IC) and you lack re‑work equipment, consider a professional repair service.
- If the regulator chip is confirmed dead and replacement isn’t feasible, evaluate whether the device cost justifies replacement.

---

**Summary**: Power path troubleshooting breaks down the power delivery network into logical checkpoints, using simple tools and visual cues to quickly locate failures without detailed, device‑specific probing instructions.
