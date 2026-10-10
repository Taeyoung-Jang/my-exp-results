---
sources: ["summaries/session-07_2024-06-15.md"]
type: "Product"
description: "YouTube is a video‑sharing platform used for delivering 4K content online."
---

# YouTube (product)

YouTube is a web‑based video hosting and streaming service owned by Google. It is a common delivery target for creators exporting high‑resolution video, especially 4K UHD content.

## Role in Session 07 (2024‑06‑15)
The conversation recommends a specific export workflow for YouTube uploads:
- Use a **two‑step workflow** [[concepts/two-step-workflow]] where a high‑quality mezzanine master is first exported (ProRes 422 or DNxHR HQX) [[concepts/mezzanine-master]].
- The mezzanine is then transcoded to a YouTube‑ready format using either H.264 [[entities/h264]] or H.265/HEVC [[entities/hevc]].
- Recommended settings include:
  - Container: MP4
  - Resolution: 3840 × 2160, 23.976 fps
  - Bit depth: 8‑bit for H.264, 10‑bit for H.265
  - VBR target: 50–55 Mbps (H.264) or 28–35 Mbps (H.265)
  - Keyframe interval: ~2 seconds
  - 2‑pass encoding enabled for H.264, optional for H.265
  - CABAC on (default for both codecs)
- Audio: AAC, 48 kHz, 320 kbps.

These settings aim to balance visual quality (including retained film grain) with file size constraints suitable for YouTube’s processing pipeline.

## Related Tools
- **Adobe Media Encoder** [[entities/adobe-media-encoder]] and **HandBrake** [[entities/handbrake]] are cited as possible encoders for the second‑pass compression step.

## Links to Documentation
- Summary of the session: [[summaries/session-07_2024-06-15]]
- Export‑settings guidance: [[concepts/export-settings]]

---
*This page was generated based on the session‑07 discussion and follows the wiki’s entity schema.*