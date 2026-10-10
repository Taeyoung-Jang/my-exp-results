---
type: "Concept"
sources: ["summaries/session-34_2025-03-14.md"]
description: "Option spreads that cap maximum loss while defining potential profit."
---

# Defined‑Risk Option Spreads

**Type:** Concept
**Description:** Option strategies that limit loss to a known amount while providing a bounded upside, making them suitable for beginners and risk‑averse traders.

---

## Overview
Defined‑risk spreads are combinations of long and short option contracts that create a position with a **maximum loss** known at entry. The most common types are:
- **Debit spreads** (e.g., bull call spread) – you pay a net premium; loss is limited to that premium.
- **Credit spreads** (e.g., bear call spread) – you receive a net credit; loss is limited to the width of the spread minus the credit received.

Both structures trade off **potential profit** for **risk certainty**, which helps new traders avoid the unlimited downside of naked options.

---

## How They Work
1. **Two‑leg construction** – One option is bought and another is sold at a different strike but same expiration.
2. **Cost vs. credit** – If the bought leg costs more than the sold leg, the spread is a **debit spread**. If the sold leg brings in more premium, the spread is a **credit spread**.
3. **Maximum loss** – Fixed at the net premium paid (debit) or the spread width minus the credit received (credit).
4. **Maximum gain** – Fixed at the difference between strikes minus any net premium paid (debit) or limited to the credit received (credit).

---

## Benefits for Small Accounts
- **Defined risk** aligns with the advice from [[summaries/session-34_2025-03-14]]: keep exposure tiny and know the worst‑case loss.
- **Lower capital requirement** – Spreads usually cost less than buying a naked option outright because the short leg offsets part of the premium.
- **Learning tool** – Managing two legs forces traders to consider how **[[concepts/options-leverage]]**, **[[concepts/options-time-decay]]**, and **volatility** interact.

---

## Choosing Parameters
- **Expiration** – Longer expirations reduce **theta** (time‑decay) pressure, giving the trade more breathing room.
- **Strike spacing** – Wider spacing increases potential profit but raises the net cost; tighter spacing is cheaper but caps upside sooner.
- **Greeks** – Track **delta** for directional sensitivity, **theta** for decay, and **vega** for volatility impact. These help you tell if the spread is behaving “normally” versus suffering from an IV crush.

---

## Common Pitfalls
- Expecting unlimited upside (the upside is capped by the spread width).
- Ignoring **theta**; even defined‑risk spreads lose value as expiration nears.
- Overlooking **vega**; a drop in implied volatility can erode the spread’s value even when the underlying is flat.
- Selecting strikes too close to expiration, which makes the trade overly sensitive to small price moves.

---

## Related Concepts
- [[concepts/options-leverage]] – explains how a small premium controls a larger notional.
- [[concepts/options-time-decay]] – describes the theta drag that affects all option positions.
- [[concepts/behavioral-finance-guardrails]] – broader discipline of keeping risk low and emotions in check.
- [[concepts/risk-tolerance-testing]] – assessing personal risk appetite before selecting spread width and size.

---

*This concept page draws primarily from the discussion in [[summaries/session-34_2025-03-14]], which introduced debit and credit spreads as beginner‑friendly, defined‑risk strategies.*