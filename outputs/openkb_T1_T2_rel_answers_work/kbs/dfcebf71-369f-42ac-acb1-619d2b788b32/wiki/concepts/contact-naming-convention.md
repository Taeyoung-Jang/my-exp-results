---
type: "Concept"
sources: ["summaries/session-35_2025-02-12.md"]
description: "A systematic naming scheme for caregiver contacts that clarifies purpose at a glance."
---

# Contact Naming Convention

**Definition**: A consistent pattern for labeling phone‑book entries related to caregiving, using a prefix (e.g., “Mom – …”) followed by the role or department, so the caller’s relevance is immediately obvious on the lock screen or in notifications.

## Why It Matters
- Enables rapid visual identification when a call or message appears, reducing decision fatigue.
- Works hand‑in‑hand with [[concepts/focus-mode-setup]] on iPhone, allowing the Focus list to filter by these clearly‑named contacts.
- Supports the "allow repeated calls" safety net described in [[concepts/repeated-calls-emergency-handling]].

## Core Structure
```
Mom – <Category> <Detail>
```
- **Category**: Clinic, Pharmacy, Home Health Agency, Emergency/Local, Family, etc.
- **Detail**: Specific function or line (Main, Nurse, After Hours, Refill, On‑Call, etc.)

### Example Prefixes
| Category | Sample Names |
|----------|--------------|
| Clinic | `Mom – Clinic Main`, `Mom – Clinic Nurse`, `Mom – Clinic Callback` |
| Pharmacy | `Mom – Pharmacy Main`, `Mom – Pharmacy Refill`, `Mom – Pharmacy Text` |
| Home Health Agency | `Mom – Home Health Main`, `Mom – Home Health Scheduler`, `Mom – Home Health On‑Call` |
| Emergency/Local | `Mom – Hospital Main`, `Mom – Hospital ER`, `Local – Police Non‑Emergency` |
| Family (urgent) | `Mom – Jane` (where *Jane* is the family member) |

## Implementation Steps (from [[summaries/session-35_2025-02-12]])
1. **Create contacts** in the iPhone address book using the above naming pattern.
2. **Group them** into Favorites or a dedicated group so they appear at the top of the contacts list.
3. **Add the contacts** to the allowed list of a custom Focus (e.g., *Caregiving*) so calls/texts from these numbers bypass silencing.
4. **Enable "Allow Repeated Calls"** to catch any unforeseen numbers from medical offices.
5. **Mute non‑essential group chats** (e.g., the aide’s group thread) while keeping direct messages allowed.

## Benefits
- **Speed**: Instantly know whether a call is about the clinic, pharmacy, or emergency without opening the contact.
- **Safety**: Reduces the chance of missing critical calls because the name itself signals priority.
- **Simplicity**: One consistent rule works across all caregiving contacts, keeping the phone organized.

## Related Concepts and Entities
- [[concepts/focus-mode-setup]] – configuring iPhone Focus with allowed contacts.
- [[concepts/repeated-calls-emergency-handling]] – using repeated‑call logic for unknown numbers.
- [[entities/clinic]], [[entities/pharmacy]], [[entities/home-health-agency]], [[entities/hospital]], [[entities/non-emergency-police]] – typical sources of contact numbers.
- [[entities/ios]], [[entities/iphone]] – platforms where this naming convention is applied.
