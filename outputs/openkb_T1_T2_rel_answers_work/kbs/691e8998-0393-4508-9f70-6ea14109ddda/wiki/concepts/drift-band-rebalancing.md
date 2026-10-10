---
type: "Concept"
sources: ["summaries/session-40_2024-06-15.md"]
description: "A rule that triggers portfolio rebalancing when allocations drift beyond a set percentage band."
---

# Drift‑Band Rebalancing

**Definition**

Drift‑Band Rebalancing is a portfolio management technique that initiates corrective trades when the weight of any asset class, sleeve, or individual position moves more than a predefined number of percentage points away from its target allocation. The drift band acts as a tolerance range, allowing natural market fluctuations while preventing the portfolio from unintentionally drifting into a riskier composition.

**Key Elements**

- **Target Allocation** – The desired mix of core ETFs, satellite stocks, and a crypto sleeve, often defined in a [[concepts/core-satellite-allocation]] framework.
- **Drift Threshold** – A common trigger is a ±5 % deviation from the target weight for any sleeve (e.g., core, satellite, crypto). This number can be adjusted based on the investor’s risk tolerance and monitoring frequency.
- **Frequency** – The rule is applied continuously, but actual trades are typically executed on a periodic schedule (e.g., monthly) or when a breach occurs.
- **Interaction with Contributions** – New cash inflows (e.g., a $2 k monthly contribution) are first directed to under‑weighted allocations, which can naturally bring the portfolio back within the drift band before any selling is required. This approach aligns with [[concepts/contribution-driven-rebalancing]].

**Implementation Steps**

1. **Define the Target Mix** – Set percentages for the core ETF basket, satellite positions, and crypto sleeve.
2. **Establish the Drift Band** – Choose a band (commonly 5 % points) for each sleeve. For example, the core ETF sleeve might be allowed to vary between 60 % and 70 % of total assets.
3. **Monitor Regularly** – Review portfolio weights at least monthly. If any sleeve exceeds its band, flag it for rebalancing.
4. **Rebalance Using Contributions** – Deploy new monthly contributions to under‑weighted areas until the drift is resolved. If contributions alone are insufficient, execute modest trades to restore balance.
5. **Annual Full Check‑In** – Conduct a comprehensive rebalance once a year to ensure all positions are aligned with the long‑term strategy.

**Benefits**

- **Risk Control** – Prevents unintended concentration and keeps the portfolio within the investor’s risk‑assessment parameters [[concepts/risk-assessment]].
- **Efficiency** – Limits trading frequency, reducing transaction costs and tax impact.
- **Behavioral Discipline** – Provides a clear, rule‑based guardrail that mitigates emotional decisions.

**Related Concepts**

- [[concepts/contribution-driven-rebalancing]] – Leveraging new cash flows to correct drift.
- [[concepts/position-sizing]] – Setting per‑position caps that complement drift‑band limits.
- [[concepts/risk-assessment]] – Evaluating overall portfolio risk to choose appropriate drift thresholds.

**Source**

The guidelines for Drift‑Band Rebalancing are drawn from the investment policy discussion in [[summaries/session-40_2024-06-15]].