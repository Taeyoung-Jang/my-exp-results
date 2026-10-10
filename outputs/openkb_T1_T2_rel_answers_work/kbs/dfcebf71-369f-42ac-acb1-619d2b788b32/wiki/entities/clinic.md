---
sources: ["summaries/session-35_2025-02-12.md"]
type: "Organization"
description: "Medical office whose numbers are central to the caregiver’s contact system"
---

# Clinic

**Type:** Organization

**Related summary:** [[summaries/session-35_2025-02-12]]

## Overview
The *Clinic* refers to the medical practice that provides primary and specialty care for the user’s mother. In the caregiving workflow described in session‑35, the clinic is a critical source of urgent and routine communications (appointment reminders, test results, medication questions, after‑hours triage).

## Key Facts from Session‑35
- The caregiver is advised to collect **all** telephone lines the clinic might use:
  - Main office number
  - Nurse/triage line
  - Appointment callback line
  - After‑hours service line
  - Lab or results line
- Each number should be saved under a **single contact** named with a clear prefix, e.g., `Mom – Clinic Main`, `Mom – Clinic Nurse`, etc., following the [[concepts/contact-naming-convention]].
- Because iOS does not support a generic “medical office” filter, grouping the numbers under one contact ensures that any call from the clinic will be allowed in the custom [[concepts/focus-mode-setup]] "Caregiving" Focus.
- The caregiver relies on the **Allow Repeated Calls** feature (see [[concepts/repeated-calls-emergency-handling]]) to catch any unexpected numbers the clinic might use.

## Suggested Contact Strategy
1. **Create a unified contact** titled `Mom – Clinic`.
2. **Add multiple phone entries** for each of the lines listed above.
3. **Add this contact to the allowed list** in the iPhone Focus mode so calls and texts bypass silencing.
4. **Enable repeated‑calls handling** to capture stray numbers that are not explicitly saved.

## Naming Convention
The recommended naming pattern is `Mom – [Role/Department]`. This aligns with the broader [[concepts/contact-naming-convention]] used for other care‑related contacts (pharmacy, home‑health agency, emergency services).

## Integration with iPhone Focus
- The caregiver creates a custom Focus (e.g., *Caregiving*) on an [[entities/iphone]] running [[entities/ios]].
- The Clinic contact is added to the **Allowed People** list.
- The Focus is scheduled for evening/night hours to minimize interruptions while still letting the clinic’s urgent calls through.

## Related Entities
- [[entities/home-health-agency]] – another care‑related organization with similar contact‑grouping guidance.
- [[entities/pharmacy]] – also saved under the `Mom – Pharmacy …` naming scheme.
- [[entities/hospital]] – listed under the emergency contacts section.
- [[entities/non-emergency-police]] – part of the broader emergency/local contact set.

---
*This entity page captures the role of the Clinic in the caregiving system outlined in the session‑35 summary.*