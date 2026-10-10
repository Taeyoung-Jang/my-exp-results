---
sources: ["summaries/session-39_2025-03-14.md"]
type: "Organization"
description: "Stripe is a payment‑processing organization used for direct software subscription billing."
---

## Stripe

Stripe is a financial technology company that provides payment‑processing services for online businesses, including recurring subscription billing.

### Role in subscription management
- In **[[summaries/session-39_2025-03-14]]**, Stripe is mentioned as a billing processor that indicates a subscription is paid **directly by the vendor** rather than through an app store.
- Recognizing a transaction description that includes "Stripe" helps users apply the **[[concepts/subscription_auditing]]** workflow to identify the source of a charge.

### How Stripe appears in charge verification
1. **Transaction clue** – The bank statement line may contain the word "Stripe".
2. **Source identification** – This signals a direct‑vendor subscription, prompting the user to log into the vendor’s website (e.g., an **[[entities/office-suite]]**) to check plan details and renewal dates.
3. **Cross‑checking** – If the description does not mention Apple or Google, Stripe becomes the likely processor, guiding the user toward the appropriate account.

### Related concepts
- **[[concepts/annual_renewal_detection]]** – Stripe‑tagged charges can be searched in email or statements to surface hidden annual renewals.
- **[[concepts/recurring_payment_tracking]]** – Including Stripe‑processed subscriptions in a master list (spreadsheet, app, or calendar) ensures they are tracked consistently.

### Additional context
- Stripe competes with other processors such as **[[entities/paddle]]** for handling subscription payments.
- While Stripe handles the payment gateway, the actual service (e.g., an office suite) remains the product the user subscribes to.

---
*This page aggregates the information about Stripe that appears in the session‑39 discussion and connects it to broader subscription‑management concepts.*