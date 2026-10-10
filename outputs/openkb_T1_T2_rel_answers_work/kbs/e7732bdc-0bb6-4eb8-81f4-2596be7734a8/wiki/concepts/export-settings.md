---
type: "Concept"
sources: ["summaries/session-31_2025-03-14.md", "summaries/session-07_2024-06-15.md"]
description: "Guidelines for choosing codecs, bitrate, resolution, and related parameters when exporting video."
---

# Export Settings

**Definition**: The set of decisions about codec, bitrate, resolution, color depth, audio format, container, and encoding options that determine the quality, file size, and render performance of a final video export.

---

## Core Elements

| Element | Typical Choices | Impact |
|---|---|---|
| **Codec** | ProRes, DNxHR (mezzanine); H.264, H.265/HEVC (delivery) | Determines compression efficiency, hardware support, and rendering speed. |
| **Bitrate** | Variable bitrate (VBR) target & max values (e.g., 40‑60 Mbps for H.264 4K) | Controls file size vs. visual fidelity; VBR adapts to scene complexity. |
| **Resolution & Frame Rate** | Preserve source (e.g., 3840×2160 at 23.976 fps) | Keeps visual fidelity; changing it can increase processing load. |
| **Bit Depth & Chroma Subsampling** | 8‑bit/4:2:0 for H.264, 10‑bit/4:2:0 for H.265, 10‑bit/4:2:2 for ProRes/DNxHR | Affects gradient smoothness and color grading headroom. |
| **Audio** | PCM 48 kHz 24‑bit (mezzanine) or AAC 48 kHz 320 kbps (delivery) | Determines audio quality and compatibility. |
| **Container** | MOV for archival mezzanine, MP4 for web delivery | Influences codec support and metadata handling. |
| **Encoding Options** | 2‑pass, CABAC, keyframe interval (≈2 s) | Improves bitrate control and streaming stability. |

---

## Best‑Practice Workflow (from [[summaries/session-07_2024-06-15]])

1. **Match source settings** – Keep the original resolution, frame rate, and color space to avoid unnecessary recompression.
2. **Select a mezzanine codec** – Use a high‑quality, low‑compression codec (ProRes or DNxHR) for the intermediate master. This speeds up the first render and prevents crashes on modest hardware.
3. **Create a delivery encode** – After the mezzanine is produced, re‑encode to the delivery codec (H.264 or H.265) using appropriate VBR targets, 2‑pass, and CABAC for efficient streaming.
4. **Optimize system resources** – Export to a fast SSD, close other applications, and use proxy/optimized media during editing.

---

## Related Concepts

- [[concepts/mezzanine-master]] – The high‑quality intermediate file used in a two‑step export.
- [[concepts/two-step-workflow]] – The overall process of separating render and compression stages.

---

## Associated Entities

- [[entities/prores]] – Apple’s ProRes codec, commonly used for mezzanine masters.
- [[entities/dnxhr]] – Avid’s DNxHR codec, the Windows counterpart to ProRes.
- [[entities/h264]] – H.264 codec, standard for web delivery.
- [[entities/hevc]] – H.265/HEVC codec, offers better compression at the same quality.
- [[entities/adobe-media-encoder]] – A popular tool for the second‑pass encoding step.
- [[entities/handbrake]] – Free encoder often used for final delivery.
- [[entities/youtube]] – Primary platform for the described delivery format.

---

## Practical Checklist (excerpt)

- **Mezzanine (ProRes/DNxHR)**: MOV/MXF, 3840×2160, 23.976 fps, 10‑bit, 4:2:2, PCM 48 kHz 24‑bit.
- **Delivery (H.264)**: MP4, High profile Level 5.2, 8‑bit, 4:2:0, VBR 50‑55 Mbps, 2‑pass, CABAC on.
- **Delivery (H.265)**: MP4, Main10, 10‑bit, 4:2:0, VBR 28‑35 Mbps, optional 2‑pass, CABAC on.

---

*This concept page synthesizes the export guidance presented in the session‑07 summary and serves as a reference for configuring high‑resolution video exports.*

See also: [[summaries/session-31_2025-03-14]]