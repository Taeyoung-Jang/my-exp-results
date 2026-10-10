---
type: "Concept"
sources: ["summaries/session-40_2025-06-15.md", "summaries/session-10_2024-06-15.md"]
description: "Standardized USPS address format including unit, ZIP+4, and official abbreviations."
---

# USPS‑Formatted Address

**Definition**: A USPS‑formatted address follows the United States Postal Service's official standards for street address layout, unit designation, city/state placement, and ZIP+4 code, ensuring reliable mail delivery and consistent data validation across vendors.

---

## Core Elements
1. **Recipient Line** – Full name or business name.
2. **Street Address** – House number, street name, and optional unit/apartment number (e.g., `Apt 4B`).
3. **City, State, ZIP+4** – City name, two‑letter state abbreviation, five‑digit ZIP followed by an optional four‑digit extension (ZIP+4) for precise routing.
4. **Formatting Rules** – All caps, standardized abbreviations (e.g., `ST` for Street, `APT` for Apartment), and a single space before the ZIP+4.

These elements were highlighted in the **address health‑check** guidance from [[summaries/session-10_2024-06-15]], where the conversation emphasized creating a *single authoritative version* of the address using the USPS lookup.

---

## Why It Matters
- **Mail Delivery Reliability** – USPS uses the ZIP+4 and exact unit to route mail to the correct carrier route.
- **Data Consistency Across Services** – Vendors like [[entities/amazon]] and [[entities/paypal]] often auto‑format addresses; comparing their stored version against a USPS‑formatted reference reveals structural mismatches such as missing unit numbers or truncated ZIP+4.
- **Risk Management** – In an [[concepts/address-audit]] or [[concepts/address-risk-prioritization]] process, the USPS‑formatted address serves as the *ground truth* for detecting harmful changes.

---

## Obtaining the USPS‑Formatted Version
1. **Use the USPS ZIP Code Lookup tool** – Enter the street address; the service returns the official, all‑caps address with ZIP+4.
2. **Copy Exactly** – Preserve spacing, punctuation, and capitalization; paste the result verbatim into the "USPS‑Verified Address" column of your audit template.
3. **Validate Unit Presence** – Ensure the unit/apartment identifier appears (e.g., `UNIT 5`, `APT 5`).

---

## Application in the Session‑10 Checklist
- The conversation recommends **starting every audit with the USPS‑verified address** as a reference point.
- When comparing vendor records, mark mismatches where the unit or ZIP+4 is omitted as "Needs correction"; purely cosmetic differences (punctuation, abbreviation) can be flagged as "Formatting only."
- For high‑risk accounts (billing or legal notices), the integrity of the USPS‑formatted address is critical, tying directly into [[concepts/address-risk-prioritization]].

---

## Related Concepts
- [[concepts/address-audit]] – systematic review process that relies on the USPS‑formatted address as baseline.
- [[concepts/address-risk-prioritization]] – prioritizing accounts based on the importance of correct address data.
- [[entities/usps]] – the agency that defines the formatting standards.
- [[entities/zip-plus-4]] – the extended ZIP code component essential for precise routing.


See also: [[summaries/session-40_2025-06-15]]