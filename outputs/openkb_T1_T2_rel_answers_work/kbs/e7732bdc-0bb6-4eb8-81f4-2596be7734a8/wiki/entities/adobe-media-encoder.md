---
sources: ["summaries/session-07_2024-06-15.md"]
type: "Product"
description: "Adobe Media Encoder is a video encoding application for batch rendering and format conversion."
---

# Adobe Media Encoder

Adobe Media Encoder (AME) is a **product** that provides fast, automated transcoding of video projects into a wide range of delivery formats. It integrates tightly with Adobe Creative Cloud apps (e.g., Premiere Pro, After Effects) and supports both **[[concepts/export-settings]]** and the **[[concepts/two-step-workflow]]** recommended for high‑resolution 4K exports.

## Role in the Session‑07 Workflow
- In the **two‑step workflow** described in [[summaries/session-07_2024-06-15]], AME is suggested as one of the dedicated encoders for the second‑pass compression stage.
- It can ingest the mezzanine master (e.g., ProRes or DNxHR) and output delivery formats such as **[[entities/h264]]**, **[[entities/hevc]]** (HEVC), or other codecs required for platforms like **[[entities/youtube]]**.
- AME allows configuration of **variable bitrate (VBR)** targets, two‑pass encoding, keyframe intervals, and CABAC settings, matching the checklist provided in the session summary.

## Key Features Highlighted
- **Batch Queueing** – Process multiple mezzanine masters sequentially or in parallel.
- **Preset Support** – Includes presets for YouTube, H.264, H.265, and custom export settings.
- **Hardware Acceleration** – Utilizes GPU encoding when available, improving render performance on limited hardware.
- **Audio Handling** – Supports PCM, AAC, and other audio codecs, preserving the 48 kHz 24‑bit PCM settings from the mezzanine master.

## Related Entities
- **[[entities/prores]]** – Common mezzanine codec used before AME processing.
- **[[entities/dnxhr]]** – Alternative mezzanine codec mentioned alongside ProRes.
- **[[entities/handbrake]]** – Another encoder option for the second‑pass step.

---
*This page aggregates the information about Adobe Media Encoder as it appears in the session‑07 document.*