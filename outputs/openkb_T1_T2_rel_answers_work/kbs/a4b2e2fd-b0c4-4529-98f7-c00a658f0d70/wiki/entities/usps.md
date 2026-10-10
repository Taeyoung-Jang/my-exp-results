---
sources: ["summaries/session-10_2024-06-15.md"]
type: "Organization"
description: "The United States Postal Service (USPS) is the U.S. national mail carrier and address authority."
---

# United States Postal Service (USPS)

The United States Postal Service (USPS) is the federal agency responsible for providing postal service in the United States, maintaining the official addressing standards, and offering services such as mail‑forwarding and ZIP+4 verification.

## Role in Address Management
- **Official address verification** – USPS supplies the authoritative, [[concepts/usps-formatted-address]] that includes correct street formatting, unit numbers, and the ZIP+4 code.  The session‑10 document advises using the USPS lookup as the single source of truth for an [[concepts/address-audit]].
- **Mail‑forwarding service** – When moving, USPS can forward mail for a configurable buffer period.  Although the user in the session is not moving, the recommendation to enable forwarding before and after a move originates from USPS capabilities.
- **ZIP+4 support** – The ZIP+4 extension (e.g., 12345‑6789) is managed by USPS and is crucial for precise delivery and for preventing mismatches in vendor records.  The entity [[entities/zip-plus-4]] represents this component.

## Relevance to Session 10
The conversation in [[summaries/session-10_2024-06-15]] highlights USPS in two main ways:
1. **Reference address source** – Users are instructed to obtain the exact, USPS‑verified address and compare it against the address stored in each account as part of an [[concepts/address-audit]].
2. **Mail‑forwarding buffer** – For those who do move, USPS’s forwarding service is recommended to create a safety window that prevents lost mail.

## Key Services Mentioned
- **Address lookup** – online tool to confirm correct formatting and retrieve ZIP+4.
- **Mail forwarding** – temporary redirection of incoming mail to a new address.
- **Change‑of‑address processing** – official filing that updates a payer’s legal mailing address.

## Related Entities and Concepts
- [[entities/usps]] – the same agency, referenced elsewhere in the wiki.
- [[entities/amazon]], [[entities/paypal]] – examples of vendors whose address records should be validated against the USPS‑verified format.
- [[concepts/address-risk-prioritization]] – the practice of ranking accounts (billing, legal, shipping) for audit urgency, where USPS‑validated data is the baseline.

---
*This page consolidates information about the United States Postal Service as it appears in the address‑audit workflow discussed in the session‑10 summary.*