---
sources: ["summaries/session-33_2025-08-15.md"]
type: "Product"
description: "Windows UI for per‑app GPU preference and power‑plan integration."
---

# Windows Graphics Settings

**Windows Graphics Settings** is a built‑in Windows interface (System → Display → Graphics) that lets users control which GPU an application uses and adjust related power settings.

## Key Facts from Session 33 (2025‑08‑15)
- **Per‑app GPU assignment** – Users can set Photoshop, Premiere, Blender, etc. to *High performance* to force the discrete GPU, preventing the system from defaulting to the integrated graphics (iGPU). This is a primary tactic for avoiding the "GPU 0" stickiness issue described in the upgrade checklist.
- **Integration with the GPU upgrade workflow** – The setting is referenced in the [[concepts/gpu-upgrade-checklist]] as a step after confirming driver installation and BIOS configuration.
- **Interaction with Quick Sync** – While the Windows Graphics Settings forces the dGPU for 3‑D workloads, the iGPU remains available for hardware‑accelerated video encoding via [[entities/intel-quick-sync]]. Users can keep the iGPU enabled for Quick Sync while still routing display output through the dGPU.
- **Verification of display routing** – Combined with Task Manager’s Performance tab, the Settings helps confirm that monitors are driven by the intended GPU, complementing the process described in [[concepts/display-connection-verification]].
- **Power‑plan influence** – Setting the app to *High performance* also nudges Windows to keep the dGPU in an active power state, reducing throttling.

## Related Concepts and Entities
- [[concepts/gpu-upgrade-checklist]] – Overall checklist for validating a GPU upgrade.
- [[concepts/display-connection-verification]] – How to confirm which GPU drives each monitor.
- [[concepts/quick-sync-utilization]] – Using Intel Quick Sync alongside a discrete GPU.
- [[entities/intel-quick-sync]] – The iGPU‑based video encoder leveraged in mixed‑GPU setups.
- [[summaries/session-33_2025-08-15]] – Source session containing the detailed guidance.
