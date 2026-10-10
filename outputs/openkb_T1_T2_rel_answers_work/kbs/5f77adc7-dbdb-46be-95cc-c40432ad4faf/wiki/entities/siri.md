---
sources: ["summaries/session-31_2025-02-15.md"]
type: "Product"
description: "Apple's voice assistant product for on‑device processing and automation."
---

# Siri (product)

Siri is Apple’s voice‑activated personal assistant that runs on iOS devices. In the context of the **developer beta** discussed in [[summaries/session-31_2025-02-15]], Siri’s on‑device processing is highlighted as a feature to **keep enabled** to retain on‑device transcription capabilities.

## Key points from the session
- **On‑device processing**: Essential for the new transcription feature; disabling it would break the primary reason for installing the beta.
- **Interaction with automation**: Works together with the Shortcuts app (see [[entities/shortcuts]]) to trigger automations based on voice commands.
- **Performance considerations**: Listed in the beta performance checklist under "Leave these on" to ensure the beta remains usable without sacrificing the transcription and automation benefits.

## Related concepts and entities
- Decision to install a beta is guided by [[concepts/beta_software_decision]] and [[concepts/upgrade_decision_criteria]].
- Troubleshooting beta issues, such as battery drain or crashes, falls under [[concepts/beta_troubleshooting]].
- Optimising beta performance, including which services to keep on, is covered by [[concepts/beta_performance_optimizations]].
- Siri often interacts with iCloud Drive (see [[entities/icloud-drive]]) for storing shortcut data.

## Practical advice for beta users
1. **Do not disable Siri/on‑device processing** when tweaking background settings; this preserves transcription.
2. Pair Siri with enabled Shortcuts to maintain automation workflows.
3. Monitor battery and heat; if issues arise, follow the broader [[concepts/beta_troubleshooting]] steps before considering a rollback.
