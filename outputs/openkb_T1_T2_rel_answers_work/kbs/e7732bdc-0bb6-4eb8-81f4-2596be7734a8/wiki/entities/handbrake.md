---
sources: ["summaries/session-07_2024-06-15.md"]
type: "Product"
description: "HandBrake is a free, open‑source video transcoder for converting media files."
---

# HandBrake

HandBrake is a free, open‑source video transcoding **product** that supports a wide range of codecs, including H.264 and H.265 (HEVC). It is commonly used for the second‑pass compression step in a [[concepts/two-step-workflow]] when exporting high‑resolution video projects.

## Role in Session 07 (2024‑06‑15)
In the **session‑07_2024-06-15** discussion, HandBrake was recommended alongside other encoders such as [[entities/adobe-media-encoder]] for the final delivery encode. The workflow suggested exporting a high‑quality mezzanine master (using [[entities/prores]] or [[entities/dnxhr]]) and then feeding that master into HandBrake to produce a YouTube‑ready MP4 file.

## Key Features Highlighted
- **Codec support**: Handles both [[entities/h264]] and [[entities/hevc]] (HEVC) encoding, allowing creators to choose H.264 for broader compatibility or H.265 for better compression efficiency.
- **Variable Bitrate (VBR) presets**: Enables the target and maximum bitrate ranges outlined in the checklist (e.g., 28‑35 Mbps target for H.265, 50‑55 Mbps target for H.264).
- **Two‑pass encoding**: Optional but recommended for H.264 to achieve more predictable bitrate control, matching the advice in the session summary.
- **Container output**: Produces MP4 files suitable for [[entities/youtube]] uploads.

## Typical Settings (as per the session checklist)
| Setting | Recommended Value |
|---|---|
| **Container** | MP4 |
| **Codec** | H.264 or H.265 (HEVC) |
| **Profile / Level** | High / 5.2 for H.264; Main10 for H.265 |
| **Bit depth** | 8‑bit for H.264, 10‑bit for H.265 |
| **Chroma subsampling** | 4:2:0 |
| **VBR target** | 50‑55 Mbps (H.264) or 28‑35 Mbps (H.265) |
| **VBR max** | 75‑90 Mbps (H.264) or 40‑50 Mbps (H.265) |
| **Keyframe interval** | 2 seconds |
| **2‑pass** | On for H.264, optional for H.265 |
| **CABAC** | Enabled |
| **Audio** | AAC 48 kHz, 320 kbps |

These parameters were derived from the checklist provided in [[summaries/session-07_2024-06-15]].

## Related Concepts and Entities
- [[concepts/export-settings]] – General guidance on choosing codecs, bitrate, and resolution.
- [[concepts/mezzanine-master]] – The intermediate high‑quality file that HandBrake receives for final compression.
- [[entities/prores]] and [[entities/dnxhr]] – Codecs recommended for creating the mezzanine master.
- [[entities/youtube]] – Target platform for the HandBrake‑encoded output.

---
*This page aggregates the information relevant to HandBrake as it appears in the session‑07 discussion.*