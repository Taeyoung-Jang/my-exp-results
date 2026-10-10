---
type: "Concept"
sources: ["summaries/session-39_2025-02-15.md", "summaries/session-05_2024-06-15.md"]
description: "A tri‑level flag system for quickly assessing app privacy and quality risk."
---

# Risk Flag System

## Definition
The **Risk Flag System** is a simple tri‑level risk assessment method used to quickly judge the long‑term viability and privacy safety of mobile applications. It assigns a **Pass (green)**, **Yellow (caution)**, or **Red (reject)** label to each evaluation criterion.

## Origin
The system originates from the app‑evaluation scorecard presented in [[summaries/session-05_2024-06-15]]. It was further refined by the quick mental checklist introduced in [[summaries/session-39_2025-02-15]], which emphasizes fast pre‑install trust checks and a “deny‑first” permission strategy.

## How It Works
For each check (e.g., update history, privacy policy, permissions, trust signals), the evaluator determines:
- **Pass (green)** – The app meets the ideal standard (e.g., updated within the last 3 months, clear privacy policy, only necessary permissions, trustworthy reviews and screenshots).
- **Yellow** – The app shows minor concerns but may still be usable (e.g., last update 6‑12 months ago, generic privacy policy, a few extra permissions, mixed reviews).
- **Red** – The app exhibits a serious red flag indicating high risk (e.g., no privacy policy, unrelated or sensitive permissions, outdated UI, clear signs of spam or hype).

The system also defines a **decision cutoff**: skip installing the app if it accumulates **two red flags**, or **one red flag plus multiple yellows**.

## Key Criteria from the Source Documents
| Check | Pass (green) | Yellow | Red |
|-------|--------------|--------|-----|
| Update history | Updated ≤3 months ago | Updated 3‑12 months ago | Updated >12 months ago |
| Recent reviews & screenshots (trust signals) | Mostly positive recent reviews, realistic screenshots | Mixed reviews or slightly outdated UI | Many “abandoned” comments, clearly spammy or placeholder screenshots |
| Developer website / portfolio | Full site with contact info and multiple stable apps | Minimal landing page or one‑two niche apps | No site or broken link |
| Privacy policy | Clear, recent, readable | Generic / vague | Missing or shady |
| Permissions | Only necessary permissions that match core features | A few extra permissions | Unrelated or sensitive permissions |
| Dev responsiveness | Recent replies in reviews | Occasional replies | No replies for a year |
| App quality (screenshots) | Polished, up‑to‑date UI | Slightly outdated UI | Clearly abandoned UI |
| Notes‑app‑only: encryption/sync | Explicit end‑to‑end encryption or transparent sync handling | Sync mentioned but unclear | No info or suspicious cloud handling |

## Relationship to Other Concepts
- Part of the broader [[concepts/app_evaluation]] methodology.
- Implements the [[concepts/evaluation_scorecard]] structure.
- Directly tied to the **risk flag** approach described in [[concepts/risk_flag_system]].

## Practical Use
1. Open the app’s store page (e.g., on the [[entities/app_store]] or [[entities/ios]]). 
2. Run through each check, marking Pass/Yellow/Red. Use the pre‑install mental script: glance at developer name, last update date, a few reviews, and screenshots before downloading.
3. Apply the cutoff rule to decide whether to install.
4. After the first launch, deny every permission request initially. Grant only those that are clearly needed for the feature you are using; otherwise, close the app and consider uninstalling.

By standardising these quick judgments, the Risk Flag System helps users maintain a high bar for privacy and support without spending hours on research.