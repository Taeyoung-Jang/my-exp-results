---
type: "Concept"
sources: ["summaries/session-13_2024-06-15.md"]
description: "A three‑tiered system (Must, Should, Nice) for verifying address consistency across services."
---

# Prioritized Checklist

**Definition**: A structured, three‑level checklist that helps users confirm that their address and billing information are consistent across critical services, grouping them into *Must check*, *Should check*, and *Nice to check* categories.

## Purpose
The checklist supports the [[concepts/source_of_truth]] approach by providing a clear order of verification, ensuring that the most important services—those that can cause legal or financial issues—are validated first. It is especially useful for maintaining [[concepts/address_consistency]] without missing any key accounts.

## Structure
| Tier | Description | Typical Services |
|------|-------------|-------------------|
| **Must check** | Services where an incorrect address can lead to serious problems and often require extra identity verification. | Primary bank and credit card accounts, the three credit bureaus ([[entities/experian]], [[entities/equifax]], [[entities/transunion]]), [[entities/dmv]], [[entities/irs]] |
| **Should check** | Services that affect day‑to‑day billing and payments but usually involve only two‑factor authentication. | Mobile carrier, utilities, insurance providers, payroll/benefits portals, major payment hubs such as [[entities/amazon]], [[entities/paypal]], [[entities/apple]], [[entities/google]] |
| **Nice to check** | Convenience‑focused services where mismatched addresses cause minor inconveniences. | Delivery‑heavy accounts like [[entities/ups]], [[entities/fedex]], [[entities/usps]], streaming services, loyalty programs, gym memberships, smaller subscription boxes |

## Identity Verification Notes
- **Must check** items often require multi‑step verification (security questions, document upload, or strong 2FA).
- **Should check** items typically rely on two‑factor codes but rarely need document proof.
- **Nice to check** items usually need only a password or one‑time code.

## How to Use
1. **Start with the source of truth** – update your address in the primary bank or credit card account.
2. **Proceed through the tiers** – confirm each service in the *Must* group, then move to *Should*, and finally *Nice*.
3. **Leverage a password manager** – store address and payment info for autofill, making mismatches obvious.
4. **Maintain a running list** – check off each service as you verify it; revisit periodically.

## Related Concepts and Resources
- [[concepts/address_consistency]] – the broader goal of keeping address data uniform.
- [[concepts/source_of_truth]] – the foundational principle behind the checklist.
- See the original discussion in [[summaries/session-13_2024-06-15]] for the full checklist and practical tips.