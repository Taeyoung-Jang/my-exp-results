---
type: "Concept"
sources: ["summaries/session-31_2025-02-15.md"]
description: "Guidelines for evaluating whether to install a developer or public beta on a mobile device."
---

# Beta Software Decision Criteria

**Purpose**: Provide a structured approach to deciding if a mobile beta (iOS or Android) should be installed, balancing the desire for new features against potential instability.

## Core Decision Factors

1. **Risk vs. Curiosity**
   - Assess how much you value early access to features (e.g., on‑device transcription, automation shortcuts) compared to tolerance for bugs, crashes, battery drain, or overheating.
2. **Primary Use Cases**
   - If the device is critical for work, travel, or essential communications, lean toward the stable release.
3. **Backup Strategy**
   - Ensure a reliable, restorable backup exists (full device image, iCloud, or local backup) before installation.
4. **App Compatibility Check**
   - Verify that essential apps (banking, messaging, productivity) are known to work or have fallback options.
5. **Device Platform**
   - The considerations apply to both [[entities/ios]] and [[entities/android]] ecosystems, though specific feature availability may differ.

## Decision Process

| Step | Action | Considerations |
|------|--------|----------------|
| 1 | List desired new features (e.g., transcription, shortcuts). | Are they unavailable in the current stable version? |
| 2 | Evaluate personal tolerance for instability. | How many crashes or performance issues are acceptable? |
| 3 | Confirm backup method and test restore capability. | Do you have a recent iCloud or local backup? |
| 4 | Check community reports and official notes on the beta build. | Look for known blockers for essential apps. |
| 5 | Make a go/no‑go decision. | If any critical factor fails, defer to the stable release. |

## Related Concepts

- [[concepts/beta_software_decision]] – broader discussion of beta adoption rationale.
- [[concepts/upgrade_decision_criteria]] – general guidelines for OS upgrades, applicable to betas.
- [[concepts/beta_troubleshooting]] – post‑install steps if issues arise.
- [[concepts/beta_performance_optimizations]] – ways to mitigate performance impacts after a beta install.

## Source

The criteria are distilled from the conversation in [[summaries/session-31_2025-02-15]].