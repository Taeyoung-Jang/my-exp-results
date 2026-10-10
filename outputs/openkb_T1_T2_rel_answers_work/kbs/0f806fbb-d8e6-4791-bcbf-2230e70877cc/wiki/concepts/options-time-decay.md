---
type: "Concept"
sources: ["summaries/session-34_2025-03-14.md"]
description: "Theta is the rate at which an option loses value as expiration approaches."
---

# Time Decay (Theta) in Options

**Type:** Concept
**Description:** Theta measures the erosion of an option’s price over time, even when the underlying stock does not move.

---

## What is Theta?
Theta, often called *time decay*, quantifies how much an option’s premium is expected to drop each day solely because time is passing. As the expiration date gets closer, there is less opportunity for the underlying price to move in‑the‑money, so the market discounts the option’s value.

## How Theta Shows Up in Practice
- **Daily “melting”** – In a flat market, an option can lose a few cents to a few dollars each day purely from the passage of time.
- **Accelerates Near Expiration** – The decay curve steepens as the contract approaches its final days. This was highlighted in the *session‑34_2025‑03‑14* discussion, where the assistant warned that “all the moves tend to feel sharper… because the market is narrowing in on the final payout.”
- **Impact on Strategies**
  - **Long Calls/Puts** – The holder bears the full brunt of theta; the position can lose value even if the stock stays unchanged.
  - **Debit Spreads** – Because two legs are involved, the net theta is usually smaller than a naked option, but it still erodes the spread’s value, especially if the stock is stagnant.
  - **Credit Spreads** – Theta works in the trader’s favor, as the spread’s price tends to shrink over time, helping the position move toward profit.

## Relationship to Other Option Greeks
- **Delta** – Captures price sensitivity; when delta is low, theta tends to dominate daily moves.
- **Vega** – Measures volatility sensitivity. A sudden drop in implied volatility (an *IV crush*) can compound theta losses, causing the option to sag faster than the calendar alone would suggest.

## Interaction with Leverage
Options provide leverage: a small premium controls a larger notional amount. Theta therefore represents a *leveraged cost*; a modest daily loss translates into a larger percentage loss on the underlying exposure. This link is explored in [[concepts/options-leverage]].

## Managing Theta in a Small Account
1. **Choose longer expirations** to slow the decay pace.
2. **Use defined‑risk spreads** (e.g., [[concepts/defined-risk-spreads]]) to reduce net theta exposure while keeping risk capped.
3. **Monitor Greeks** daily to understand whether the move you see is driven by delta, theta, or vega.
4. **Treat each trade as a learning experiment**, focusing on how the option’s price changes over time rather than on short‑term profit.

## Example from the Source Document
> *“If the stock stays stuck at 50 for a few days, you might see your option sag from 2.00 to 1.85 to 1.70 even though nothing happened.”* – This illustrates pure theta decay in action.

---

### Related Concepts
- [[concepts/options-leverage]]
- [[concepts/defined-risk-spreads]]
- [[concepts/options-time-decay]] (this page) 

### Source
- [[summaries/session-34_2025-03-14]]
