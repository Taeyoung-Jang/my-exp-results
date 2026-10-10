---
type: "Concept"
sources: ["summaries/session-40_2025-06-15.md", "summaries/session-10_2024-06-15.md"]
description: "A systematic process for verifying and synchronizing personal address data across all accounts."
---

# Address Audit

**Definition**

An **Address Audit** is a structured review of every service, account, or system that stores a person's mailing address, comparing the stored value against an authoritative [[concepts/usps-formatted-address]] (typically the USPS‑verified version with correct unit and ZIP+4). The goal is to detect and correct unintended alterations—such as dropped unit numbers or truncated ZIP+4—while distinguishing harmless formatting differences.

---

## Why Conduct an Address Audit?

- Prevents loss of critical communications (billing statements, legal notices, tax documents).
- Avoids accidental changes that can arise from vendor auto‑formatting.
- Ensures consistency across platforms like [[entities/amazon]], [[entities/paypal]], banks, utilities, and medical portals.
- Provides a risk‑based prioritization framework so that high‑impact accounts (billing, legal) are checked first.

---

## Core Components

1. **Reference Address** – Retrieve the official address from the [[entities/usps]] lookup, including the [[entities/zip-plus-4]] and exact unit formatting.
2. **Account Inventory** – List every account where the address is stored (online shopping, financial, healthcare, subscriptions, etc.).
3. **Comparison Matrix** – For each account, capture the *exact* address shown, then evaluate:
   - Does the unit number appear?
   - Is the ZIP+4 correct?
   - Are any structural elements altered (e.g., removal of “Apt” or “#”)?
4. **Risk Prioritization** – Classify each entry by its purpose (billing, shipping, legal notices) and assign a **Risk Level** (high, medium, low) using the principles from [[concepts/address-risk-prioritization]].
5. **Vendor Behavior Log** – Note whether the service auto‑rewrites the address (e.g., Amazon dropping the unit, PayPal re‑formatting abbreviations).

---

## Recommended Template (Spreadsheet Layout)
| Column | Description |
|--------|-------------|
| **Account Name** | Service or organization (e.g., Amazon, PayPal). |
| **Address Purpose** | Billing / Shipping / Legal / Verification / All |
| **Address on File (Exact Copy)** | Literal address displayed in the account. |
| **USPS‑Verified Address** | Reference address for direct comparison. |
| **Critical Fields Intact?** | Yes/No – are unit and ZIP+4 present? |
| **Formatting Only?** | Yes/No – only punctuation/abbreviation differences. |
| **Vendor Auto‑Changes?** | Description of any silent reformatting observed. |
| **Risk Level** | High, Medium, Low (based on purpose). |
| **Last Checked** | Date of review. |
| **Notes** | Additional observations. |

---

## Process Steps
1. **Obtain the authoritative address** from [[entities/usps]] and store it as the reference.
2. **Gather accounts** and fill the template, copying the exact on‑screen address.
3. **Compare** each entry to the reference, marking status in *Critical Fields Intact?* and *Formatting Only?*.
4. **Assign risk** using the address purpose; prioritize high‑risk items for immediate correction.
5. **Correct mismatches** where structural elements are missing; ignore purely cosmetic changes.
6. **Document vendor behavior** for future reference and possible automation.
7. **Repeat** the audit periodically (e.g., quarterly) to catch any drift.

---

## Related Concepts & Entities
- [[concepts/address-risk-prioritization]] – methodology for ranking address‑related risks.
- [[concepts/usps-formatted-address]] – the standard format used as the audit baseline.
- [[entities/amazon]] – example of a vendor that may drop unit numbers.
- [[entities/paypal]] – example of a vendor that may reformat but keep ZIP+4.
- [[entities/usps]] – provider of the official address verification service.
- [[entities/zip-plus-4]] – component of the address critical for precise routing.

---

## Source
This concept is derived from the discussion in [[summaries/session-10_2024-06-15]], which provided the checklist, templates, and risk‑prioritization guidance for a personal address health check.


See also: [[summaries/session-40_2025-06-15]]