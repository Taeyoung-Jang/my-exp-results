---
type: "Concept"
sources: ["summaries/session-10_2020-05-12.md"]
description: "A streamlined invoicing method using a single tool for creating invoices and collecting payments, cutting manual effort."
---

# Low‑Friction Invoicing

**Overview**

Low‑friction invoicing is a workflow that lets freelancers generate professional invoices, share payment links, and automatically record transactions without juggling multiple apps or manual bookkeeping. The goal is to keep the invoicing and payment process so simple that it does not feel like a second job.

**Core Components**

- **Single invoicing & payment platform** – Typically a service like [[entities/stripe]] that can both create invoices and process card or bank‑transfer payments.
- **Separate business bank account** – Accounts such as [[entities/novo]] or [[entities/mercury]] keep personal and business cash separate and feed transaction data to bookkeeping tools.
- **Lightweight bookkeeping tool** – A free or low‑cost solution like [[entities/wave]] that auto‑imports transactions and learns to categorize them.

**Key Settings for Autopilot**

- Enable [[concepts/automated-payment-reminders]] in Stripe to reduce chasing late payments.
- Set up recurring invoices (covered in the source) for regular clients.
- Turn on [[concepts/automatic-transaction-categorisation]] in Wave so expenses and income are auto‑sorted after an initial training batch.
- Define default invoice terms, payment methods (card + bank transfer), and a reusable invoice template with logo and common line items.

**First‑Week Checklist (Day‑by‑Day)**

1. **Day 1 – Stripe**: create account, link business bank, enable auto‑reminders, allow card and ACH, set default terms, save template, configure recurring invoices.
2. **Day 2 – Business Bank**: open account (e.g., Novo or Mercury), set it as Stripe payout account, activate any bank‑provided auto‑categorisation.
3. **Day 3 – Wave**: create account, link both Stripe and the bank, review default categories.
4. **Day 4 – Train Wave**: categorize a small batch of recent transactions to teach the system.
5. **Day 5 – Test Workflow**: send a test invoice, confirm payment lands in Stripe and appears correctly in Wave.
6. **Day 6 – Polish**: fine‑tune line items, client list, and correct any mis‑categories.
7. **Day 7 – Hands‑off**: system ready for regular use.

**Ongoing Maintenance**

A [[concepts/weekly-maintenance-routine]] of about ten minutes each week—review the latest transactions in Wave, correct any mis‑categorisations, and verify Stripe payouts have synced—keeps the system running smoothly.

**Benefits**

- Minimal setup time (1–2 hours total).
- Automated reminders reduce late payments.
- Automatic categorisation cuts bookkeeping to a quick weekly check.
- Clear separation of personal and business finances.

**Related Concepts**

- [[concepts/automated-payment-reminders]]
- [[concepts/automatic-transaction-categorisation]]
- [[concepts/weekly-maintenance-routine]]

**Source**

The details of this approach are drawn from [[summaries/session-10_2020-05-12]].