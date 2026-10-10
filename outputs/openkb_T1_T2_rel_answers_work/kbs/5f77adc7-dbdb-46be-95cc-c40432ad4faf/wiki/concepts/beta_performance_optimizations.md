---
type: "Concept"
sources: ["summaries/session-31_2025-02-15.md"]
description: "Techniques to reduce battery drain, heat, and instability in mobile beta builds while preserving core features."
---

# Beta Performance Optimizations

**Definition**: Practical settings and routines that mitigate the side‑effects of running a developer or public beta on a mobile device—specifically battery consumption, thermal output, and app stability—without disabling the new functionality that motivated the beta install.

---

## Core Principles (derived from [[summaries/session-31_2025-02-15]])
1. **Target background load, not core features** – Keep services required for on‑device transcription and automation shortcuts active, but trim or disable ancillary background tasks.
2. **Iterative monitoring** – After each change, observe battery, temperature, and crash logs for a day to confirm the adjustment helps.
3. **Grace period for re‑indexing** – Give the OS 1‑2 hours (or a full day) of idle time post‑install to finish indexing; many early‑beta spikes subside on their own.

---

## Checklist of Optimizations
| Category | Action | Rationale |
|----------|--------|-----------|
| **Keep Enabled** | Siri/on‑device processing, Shortcuts automations, iCloud Drive, required Location Services | These powers the on‑device transcription and automation shortcuts that motivated the beta. |
| **Turn Off / Limit** | Background App Refresh for rarely‑used apps, System Analytics & Improvements, Share iPhone Analytics, Share with App Developers, "Allow Apps to Request to Track" | Reduces constant wake‑ups and network traffic that drain battery and generate heat. |
| **Adjust (Don’t Disable)** | 5G → **5G Auto** (instead of always‑on), Bluetooth scanning for non‑essential apps, Always‑On Display (lower brightness or disable), Auto‑Lock to 30 s | Maintains connectivity for needed features while limiting power‑hungry continuous radio use. |

---

## Practical Steps
1. **Backup First** – Create a full device backup (iCloud or encrypted iTunes) so you can restore if optimizations cause regressions.
2. **Apply Settings** – Follow the checklist above; most toggle locations are in Settings → **General** → **Background App Refresh**, Settings → **Privacy**, and Settings → **Cellular/Data**.
3. **Reboot** – Restart the phone to let the system re‑evaluate resource allocation.
4. **Monitor** – Use the built‑in Battery usage screen and any third‑party temperature monitor for 24‑48 hours.
5. **Iterate** – If battery drain remains high, further limit background refresh for additional apps or disable less‑critical location services.

---

## When to Roll Back (linked to [[concepts/beta_troubleshooting]])
- Repeated crashes of essential apps (banking, messaging, calls).
- Persistent heat that makes the device uncomfortable to hold.
- Battery dropping below ~15 % within a few hours of normal use despite the above tweaks.

If any of these thresholds are crossed, restore the pre‑beta backup and wait for a more stable build.

---

## Related Concepts
- [[concepts/beta_software_decision]] – Deciding whether to install a beta in the first place.
- [[concepts/beta_troubleshooting]] – How to diagnose and address issues that arise after a beta install.
- [[concepts/upgrade_decision_criteria]] – Broader factors influencing upgrade choices beyond performance.

---

*Page last updated: 2026‑10‑10*