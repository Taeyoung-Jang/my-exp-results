---
sources: ["summaries/session-10_2024-06-15.md"]
type: "Organization"
description: "Online payments platform that may auto‑format stored addresses."
---

# PayPal

**Type:** Organization

**Description:** PayPal is an online payment service that stores user billing and shipping addresses.

**Relevant context in [[summaries/session-10_2024-06-15]]:** In the address‑audit discussion, PayPal is cited as a vendor that can automatically reformat address entries, potentially dropping unit numbers or altering ZIP+4. Users are advised to paste the USPS‑verified address into PayPal’s form and verify it using the "Vendor Auto‑Changes?" column of the audit template.

**Associated concepts**
- [[concepts/address-audit]] – systematic review of stored addresses, includes PayPal as an example.
- [[concepts/address-risk-prioritization]] – evaluating the risk of address changes for billing‑critical services like PayPal.
- [[concepts/usps-formatted-address]] – the reference format against which PayPal’s stored address should be compared.

**Related entities**
- [[entities/amazon]] – another vendor mentioned for address formatting behavior.
- [[entities/usps]] – provides the official address standard.
- [[entities/zip-plus-4]] – component of the USPS‑formatted address that PayPal must retain.