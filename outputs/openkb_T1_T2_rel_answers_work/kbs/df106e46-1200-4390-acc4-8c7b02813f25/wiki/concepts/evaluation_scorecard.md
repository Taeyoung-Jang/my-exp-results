---
type: "Concept"
sources: ["summaries/session-39_2025-02-15.md", "summaries/session-05_2024-06-15.md"]
description: "A rapid checklist that grades app longevity, privacy, and support to guide install decisions."
---

# Evaluation Scorecard

**Definition**: A short, structured checklist that lets users evaluate a mobile app’s longevity, privacy, and support in under five minutes. It grades each criterion as **Pass**, **Yellow**, or **Red** and uses a simple cutoff rule to decide whether to install the app.

---

## Purpose
The scorecard operationalises the broader [[concepts/app_evaluation]] methodology by providing concrete, repeatable checks. It is designed for rapid decision‑making on both habit‑tracker and notes‑type apps, and it complements the quick mental script introduced in the "download‑first, think‑later" discussion (see [[summaries/session-39_2025-02-15]]). Together they form a practical [[concepts/pre_install_checklist]] for fast, privacy‑aware app selection.

---

## Core Structure
| Check | How to Verify Quickly | Pass | Yellow | Red |
|-------|-----------------------|------|--------|-----|
| **Update history** | App Store listing “Last updated” | ≤ 3 months | 3‑12 months | > 12 months |
| **Recent reviews** | Sort by most recent, read sentiment | Mostly positive, recent | Mixed or occasional bug complaints | Many “abandoned” comments |
| **Developer reputation** (trust signal) | Look at developer name, other apps, website | Recognised, multiple stable apps | One‑two niche apps | Single unknown app |
| **Developer website** | Follow developer link | Full site with contact info | Barebones or outdated site | No site / broken link |
| **Privacy policy** | Open from store listing | Clear, current, detailed | Generic or vague | Missing or sketchy |
| **Permissions** | View permissions (iOS: App Privacy/Data Used) | Only needed permissions | A few extra permissions | Unrelated or sensitive permissions |
| **Permission alignment** | Does each permission match a core feature? (see [[concepts/permission_red_flags]]) | All aligned | Some questionable | Major mismatches |
| **Developer responsiveness** | Review replies from developer | Recent replies | Occasional replies | No replies for a year |
| **App quality** | Screenshots & description | Polished, up‑to‑date UI | Slightly outdated UI | Clearly abandoned design |
| **Notes‑app‑only: encryption/sync** | Look for E2E or clear sync description | Explicit E2E or transparent handling | Sync mentioned but unclear | No info or suspicious cloud handling |

---

## Risk Flag System
Each criterion maps to a **risk flag**:
- **Pass** – no concern.
- **Yellow** – moderate concern; may be acceptable if other checks are strong.
- **Red** – high concern; indicates a likely problem.

The overall decision rule (derived from the source conversation) is:
- **Skip installation** if the app has **two red flags**, or **one red flag plus three or more yellows**. This simple heuristic balances privacy, support, and longevity considerations.

---

## iOS‑Specific Guidance
On iOS, permission details are found in the **App Privacy** and **Data Used** sections of the App Store listing (see [[entities/ios]]). Look for permissions that do not align with the app’s core function (e.g., location for a habit tracker, contact access for a notes app). This aligns with the [[concepts/permission_red_flags]] approach.

---

## Integration with Quick Pre‑Install Checklist
The conversational checklist from session‑39 can be used **before** applying the scorecard:
1. **Who made it?** Verify the developer (trust signal).
2. **Last update?** Check the update history criterion.
3. **Reviews & screenshots** – skimming satisfies the recent reviews and app quality rows.
4. **Red‑flag permissions?** Evaluate the Permissions and Permission alignment rows.
5. **Gut check** – if any step feels off, treat it as a Yellow or Red flag.

After installation, the "deny‑first" permission strategy described in the session complements the **Permissions** and **Permission alignment** rows of the scorecard, ensuring that only context‑needed access is granted.

---

## Application Context
The scorecard was first introduced in the conversation documented in [[summaries/session-05_2024-06-15]], where it was used to compare habit‑tracker and notes apps. The later discussion in [[summaries/session-39_2025-02-15]] added a concise mental script that maps directly onto several rows of the scorecard, making the overall evaluation process even faster.

---

## Related Concepts
- [[concepts/app_evaluation]] – the overarching framework for assessing app health.
- [[concepts/app_trust_signals]] – the set of signals (developer reputation, update cadence, reviews, etc.) that inform many scorecard rows.
- [[concepts/risk_flag_system]] – the underlying flag taxonomy that the scorecard employs.
- [[concepts/permission_red_flags]] – criteria for spotting permission mismatches.
- [[concepts/pre_install_checklist]] – the quick mental script that aligns with the scorecard.

*End of concept page.*