---
type: "Concept"
sources: ["summaries/session-13_2024-06-15.md"]
description: "Central location where address and billing info are first updated."
---

# Source of Truth

**Definition**: A single, authoritative repository for personal address and billing information that other services reference and synchronize with.

## Why It Matters

In [[summaries/session-13_2024-06-15]] the assistant recommends establishing a *source of truth* to ensure [[concepts/address_consistency]] across banks, credit bureaus, government agencies, and online platforms. By updating the address in one place first, subsequent updates become predictable and reduce the risk of missed or inconsistent records.

## Practical Implementation

1. **Choose a primary account** – Typically a main bank or credit‑card issuer because many other services pull data from financial institutions.
2. **Update the address there** – Ensure the new or verified address is correctly entered.
3. **Propagate outward** – Systematically verify and update the address in the groups defined by the [[concepts/prioritized_checklist]] (Must, Should, Nice).

## Related Entities

- [[entities/dmv]] – Government record that should be updated after the source of truth.
- [[entities/irs]] – Tax authority account that relies on the same address.
- [[entities/experian]], [[entities/equifax]], [[entities/transunion]] – Credit bureaus that need the correct address for reporting.
- [[entities/amazon]], [[entities/apple]], [[entities/google]] – Major online platforms where the address is often auto‑filled from saved payment info.

## Benefits

- **Consistency**: Reduces duplicate effort and errors across services.
- **Security**: Centralizing updates limits exposure to identity‑verification steps to a few trusted platforms.
- **Efficiency**: A short running list of services can be cross‑checked quickly after the source of truth is confirmed.

By treating a single account as the *source of truth*, users can maintain reliable [[concepts/address_consistency]] with minimal ongoing maintenance.