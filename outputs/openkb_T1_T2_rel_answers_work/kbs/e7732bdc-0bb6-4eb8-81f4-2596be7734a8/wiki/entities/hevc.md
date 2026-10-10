---
sources: ["summaries/session-07_2024-06-15.md"]
type: "Product"
description: "HEVC (H.265) is a high‑efficiency video codec for 4K delivery."
---

# HEVC (H.265)

**Type:** Product

## Overview
HEVC, also known as H.265, is a video compression standard that delivers the same visual quality as H.264 at roughly half the bitrate. It supports 10‑bit depth, Main10 profile, and is widely used for high‑resolution (e.g., 4K UHD) streaming and archival workflows.

## Key Settings from Session‑07
- **Container:** MP4
- **Profile:** Main10 (10‑bit)
- **Resolution:** 3840×2160
- **Frame rate:** 23.976 fps
- **Bit depth:** 10‑bit
- **Chroma subsampling:** 4:2:0
- **VBR target:** 28–35 Mbps
- **VBR max:** 40–50 Mbps
- **Keyframe interval:** 2 seconds
- **2‑pass:** Optional (stable encoders)
- **CABAC:** Enabled (default for HEVC)
- **Audio:** AAC 48 kHz, 320 kbps

These settings were recommended for the YouTube delivery variant in the [[summaries/session-07_2024-06-15]] document.

## Role in the Two‑Step Workflow
HEVC is used in the second pass of the [[concepts/two-step-workflow]] to create a lightweight, streaming‑ready file after an intermediate mezzanine master has been exported. The workflow separates the heavy creative render (using [[entities/prores]] or [[entities/dnxhr]]) from the final compression step, allowing systems with limited processing power to complete 4K exports reliably.

## Related Tools & Entities
- [[entities/h264]] – alternative codec often used when HEVC is not supported.
- [[entities/prores]] – recommended mezzanine master codec for the first export step.
- [[entities/dnxhr]] – another mezzanine codec option for Windows users.
- [[entities/handbrake]] – popular open‑source encoder that can produce HEVC output.
- [[entities/adobe-media-encoder]] – professional encoder capable of HEVC encoding.
- [[entities/youtube]] – primary delivery platform that accepts HEVC (HEVC‑encoded MP4) uploads.

## Related Concepts
- [[concepts/export-settings]] – guidelines for choosing bitrate, profile, and container.
- [[concepts/mezzanine-master]] – the high‑quality intermediate file that precedes HEVC encoding.

---
*Page generated based on information from the session‑07 discussion.*