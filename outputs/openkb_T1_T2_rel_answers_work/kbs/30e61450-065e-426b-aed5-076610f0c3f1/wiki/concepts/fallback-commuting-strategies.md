---
type: "Concept"
sources: ["summaries/session-34_2025-04-11.md"]
description: "A hierarchy of primary, backup, and last‑resort commuting options based on preferences and constraints."
---

# Fallback Commuting Strategies

**Definition** – A structured hierarchy that designates a *default* commuting mode, a *backup* alternative, and a *last‑resort* option, chosen according to an individual’s personality, lifestyle, and situational factors such as weather, vehicle availability, or fatigue.

## Origin
The concept is drawn from the checklist and personalized plan presented in [[summaries/session-34_2025-04-11]], where a driver‑oriented user was provided with:
1. **Default plan** – [[entities/personal-car]]
2. **Backup plan** – [[entities/ride-share]]
3. **Last‑resort plan** – [[entities/public-transit]]

## Relationship to Other Concepts
- It operationalises the **commuting preferences** captured by the questionnaire in [[concepts/commuting-preferences]].
- The selection logic follows the **mode‑recommendation matrix** described in [[concepts/mode-recommendation-matrix]], mapping answer patterns (A/B/C) to a tiered set of options.

## Key Elements
| Tier | Typical Mode | Why it fits the user |
|------|--------------|----------------------|
| **Default** | Personal car | Highest control, privacy, and predictability – aligns with dominant “A” answers (structured, solitary, convenient). |
| **Backup** | Ride‑share | Preserves door‑to‑door convenience and personal bubble without requiring the user to drive, useful when the primary mode is unavailable or undesirable. |
| **Last‑resort** | Public transit | Accepts lower control and higher exposure to crowds; activated only when both personal car and ride‑share are infeasible. |

## Scenario Applications
- **Bad weather** – Switch to the backup (ride‑share) to retain comfort while avoiding exposure.
- **Vehicle in the shop** – Backup mode steps in seamlessly, mirroring the default experience.
- **Exhaustion after work** – Backup mode again, offering a private space without the mental load of driving.

## Benefits
- **Resilience** – Guarantees a viable commute under varied conditions.
- **Psychological consistency** – Each tier preserves core preferences (privacy, predictability) as much as possible.
- **Flexibility** – Users can adapt quickly without re‑evaluating the entire questionnaire.

## Implementation Tips
1. Use the 12‑question checklist to identify the dominant answer pattern.
2. Assign the tiered modes as shown above.
3. Periodically review the hierarchy as lifestyle or city‑wide transport options evolve.

---
*See also:* [[concepts/commuting-preferences]], [[concepts/mode-recommendation-matrix]]