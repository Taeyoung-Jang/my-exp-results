---
sources: ["summaries/session-33_2025-08-15.md"]
type: "Product"
description: "Intel's hardware video encoding/decoding technology for fast H.264/H.265 processing."
---

## Intel Quick Sync

Intel Quick Sync is a hardware‑accelerated video encode and decode feature built into Intel integrated graphics (iGPU). It enables fast H.264 and H.265 encoding/decoding, often used to speed up export and playback in video‑editing applications.

### Key facts from session‑33 (2025‑08‑15)
- **Enabled by leaving the iGPU active** after a discrete GPU upgrade, allowing Premiere Pro and Media Encoder to off‑load H.264/H.265 encoding to the Intel iGPU while the discrete GPU handles 3D rendering and effects.
- **Verification**: During an export, Task Manager’s *Performance* tab shows activity on the Intel GPU’s *Video Encode* or *Video Decode* engines, confirming Quick Sync is in use.
- **Benefits**: Provides hardware‑accelerated encoding without taxing the CPU, complementing the discrete GPU’s role for effects, playback, and CUDA/OpenCL rendering.
- **Potential issues**: Some apps default to the system’s GPU 0 (often the iGPU); overriding the app’s graphics preference in windows graphics settings or the NVIDIA Control Panel ensures the iGPU is used only for encoding, while the dGPU handles rendering.

### Related concepts and entities
- [[concepts/display-connection-verification]] – checking which GPU drives each monitor.
- [[concepts/gpu-upgrade-checklist]] – includes steps to keep the iGPU enabled for Quick Sync.
- [[concepts/quick-sync-utilization]] – detailed guidance on leveraging Quick Sync in workflows.
- [[entities/adobe-premiere-pro]] – software that can use Quick Sync for hardware‑accelerated encoding.
- [[entities/nvidia]] – the discrete GPU that handles rendering alongside Quick Sync.
- [[summaries/session-33_2025-08-15]] – source document summarizing Quick Sync usage in a workstation upgrade scenario.