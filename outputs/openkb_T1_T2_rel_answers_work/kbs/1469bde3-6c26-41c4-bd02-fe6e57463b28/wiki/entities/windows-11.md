---
sources: ["summaries/session-38_2025-02-15.md"]
type: "Product"
description: "Microsoft's Windows 11 operating system for PCs."
---

# Windows 11

**Type:** Product

**Owner:** [[entities/microsoft]]

Windows 11 is the latest consumer operating system from Microsoft, designed for modern PCs. It introduces several update‑control features that are central to a stable week‑day workflow.

## Update Management in Windows 11 (as discussed in [[summaries/session-38_2025-02-15]])

- **Active Hours** – Users can define a block of time (e.g., 9 am‑5 pm) during which Windows will not automatically restart or finish installations. This is covered by the concept [[concepts/windows-active-hours]].
- **Pause Updates** – The UI offers a one‑week pause button that temporarily stops all update delivery, useful during short deadline crunches.
- **Feature‑Update Deferral** – On Windows 11 Home the true deferral option is missing; the practical approach is to simply avoid clicking the *Download and install* button on feature‑update banners. The toggle *Get the latest updates as soon as they’re available* (found under Settings → Windows Update → Advanced options) may be hidden on some Home builds.
- **Optional / Preview Updates** – These appear under *Optional updates*; skipping them prevents surprise changes. Driver updates are also listed there and can be ignored unless needed.
- **Microsoft Store Auto‑Updates** – To keep apps stable, disable automatic updates via the Store app (Profile → App Settings). This aligns with a broader [[concepts/software-update-strategy]] of manual weekend updates.

## Recommended Weekend Update Routine

1. Restart the device.
2. Open **Settings → Windows Update** and install all pending patches (including cumulative security updates).
3. Open the **Microsoft Store** and manually update apps if desired.
4. Restart again if major updates were applied.

Following this routine keeps the system secure while avoiding mid‑week disruptions.

---

*Related entities:* [[entities/windows-update]], [[entities/microsoft-store]]
