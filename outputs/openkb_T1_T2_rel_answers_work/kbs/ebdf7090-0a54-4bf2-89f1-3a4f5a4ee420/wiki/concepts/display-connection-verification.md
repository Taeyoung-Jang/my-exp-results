---
type: "Concept"
sources: ["summaries/session-33_2025-08-15.md"]
description: "Method to confirm which GPU is driving each display and detect mis‑wired monitors."
---

# Display Connection Verification

**Definition**: A set of checks to determine which graphics processor (integrated iGPU or discrete dGPU) is currently driving each connected monitor, and to identify symptoms caused by connecting a display to the wrong video output.

## Why It Matters
When a workstation receives a new discrete graphics card, monitors may still be plugged into the motherboard’s video ports. This results in the system behaving as if the new GPU is idle: sluggish UI, missing high‑refresh rates, and low GPU utilization in benchmarks. Detecting the mis‑connection early prevents wasted troubleshooting time.

## Core Verification Steps (from [[summaries/session-33_2025-08-15]])
1. **Open Windows Task Manager → Performance tab**.
2. Select each listed GPU (e.g., *GPU 0 Intel* and *GPU 1 NVIDIA*). At the top of the pane the *Displays* line shows which monitor numbers are attached to that GPU.
3. If a monitor appears only under the Intel GPU, it is physically connected to the motherboard port; move the cable to the discrete card’s HDMI/DisplayPort.
4. Confirm that after reconnection the monitor now lists under the dGPU (NVIDIA/AMD) and that the GPU shows activity when launching a graphics‑intensive app.

## Symptom Checklist
- Desktop feels “slow” despite a powerful GPU installed.
- No high‑resolution or high‑refresh‑rate options appear in Windows Display Settings.
- Task Manager shows near‑zero usage on the dGPU while the CPU spikes.
- Applications (Photoshop, Premiere, Blender) default to software rendering or report "GPU not detected."

## Quick Tools
- **Task Manager GPU monitoring** – built‑in, no extra install.
- Third‑party utilities such as **GPU‑Z** or **MSI Afterburner** can also list attached displays per GPU.
- Use the Windows Settings *System > Display* pane; each monitor’s *Advanced display settings* will show the adapter name.

## Integration with a GPU Upgrade Checklist
The verification steps are a crucial sub‑task of the broader [[concepts/gpu-upgrade-checklist]]. After confirming BIOS primary‑display selection and driver installation, run the display‑connection verification to ensure the physical wiring matches the logical configuration.

## Related Concepts
- [[concepts/gpu-upgrade-checklist]] – overall post‑upgrade health checks.
- [[concepts/quick-sync-utilization]] – may rely on the iGPU remaining enabled; correct display routing prevents accidental fallback to the iGPU for rendering.

---
*This concept consolidates the practical guidance from session‑33 on how to reliably verify monitor‑GPU assignments and avoid common pitfalls after a graphics card upgrade.*