---
type: "Concept"
sources: ["summaries/session-33_2025-08-15.md"]
description: "Using Intel Quick Sync for hardware video encoding alongside a discrete GPU."
---

# Quick Sync Utilization

**Definition**: Leveraging Intel's integrated GPU (iGPU) to perform hardware‑accelerated H.264/H.265 encoding and decoding (Quick Sync) while a discrete GPU handles 3D rendering and effects.

---

## Core Idea
Quick Sync provides a low‑power, high‑throughput video encoder that can be used in conjunction with a separate dGPU. This allows workflows such as Adobe video editing to off‑load compression to the iGPU while retaining GPU‑accelerated playback, effects, and color grading on the discrete GPU.

---

## How It Works in a Typical Workstation Upgrade
1. **Keep the iGPU enabled** in BIOS so the Intel driver can expose the Quick Sync engine.  
2. **Connect all monitors to the discrete GPU** ports to ensure the display output uses the dGPU for rendering.  
3. In **Adobe Premiere Pro** (or Media Encoder), select *Intel Quick Sync* as the hardware encoder in the export settings.  
4. Verify activity:
   - Open **Task Manager → Performance → Intel GPU** and watch the *Video Encode* engine spike during an export.
   - Simultaneously, observe the discrete GPU (e.g., NVIDIA) showing load on its 3D/Compute engines for effects and playback.
5. Force the dGPU for all GPU‑intensive apps via **Windows Graphics Settings** or the **NVIDIA Control Panel** to avoid accidental fallback to the iGPU.

---

## Benefits
- **Faster H.264/H.265 renders** with lower CPU usage compared to software encoding.
- **Energy efficiency**: Quick Sync consumes far less power than the dGPU for pure encoding tasks.
- **Parallelism**: Encoding can run on the iGPU while effects and playback run on the dGPU, maximizing overall throughput.

---

## Potential Gotchas
- Some applications default to *GPU 0* (often the iGPU). Explicitly assign the app to *High performance* in [[entities/windows-graphics-settings]] to keep it on the dGPU.
- If the iGPU is disabled in BIOS, Quick Sync is unavailable; ensure the BIOS setting aligns with desired workflow.
- Stale Intel graphics drivers can prevent Quick Sync from being detected; keep drivers up‑to‑date.

---

## Related Concepts & Entities
- [[concepts/display-connection-verification]] – checking which GPU drives each monitor.
- [[concepts/gpu-upgrade-checklist]] – overall checklist that includes enabling/disabling the iGPU.
- [[entities/intel-quick-sync]] – hardware feature leveraged.
- [[entities/adobe-premiere-pro]] – primary application that can use Quick Sync.
- [[entities/nvidia]] – typical discrete GPU used for rendering.
- [[entities/windows-graphics-settings]] – method to force app GPU selection.

---

## Source
The details above are drawn from the workstation upgrade discussion in [[summaries/session-33_2025-08-15]].