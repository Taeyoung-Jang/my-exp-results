---
type: "Concept"
sources: ["summaries/session-31_2025-03-14.md", "summaries/session-07_2024-06-15.md"]
description: "A workflow that first exports a mezzanine master, then encodes the final delivery."
---

## Two‑Step Workflow

The **Two‑Step Workflow** is a reliable export strategy for high‑resolution video projects that separates the demanding creative render from the heavy compression pass. It is especially useful when hardware resources are limited, as described in [[summaries/session-07_2024-06-15]].

### Why Use a Two‑Step Workflow?
- **Stability:** Rendering a high‑quality mezzanine master avoids crashes that can occur when encoding directly to a delivery codec.
- **Speed:** Mezzanine codecs such as [[entities/prores]] (on macOS) or [[entities/dnxhr]] (on Windows) are fast to encode and produce visually lossless files.
- **Flexibility:** The intermediate file can be re‑encoded multiple times with different delivery settings without re‑rendering the timeline.

### Core Steps
1. **Export Mezzanine Master**
   - Choose a high‑performance intermediate codec (see [[concepts/mezzanine-master]]).
   - Keep source resolution, frame rate, and bit depth unchanged.
   - Use a container like MOV for archival safety.
2. **Second‑Pass Encode for Delivery**
   - Feed the mezzanine file into a dedicated encoder such as [[entities/adobe-media-encoder]], [[entities/handbrake]], or any other tool that supports the target codec.
   - Apply the desired delivery settings (see [[concepts/export-settings]]) – e.g., H.264 for broad compatibility or HEVC/H.265 for better compression.
   - Enable optional features like 2‑pass encoding, CABAC, and appropriate keyframe intervals for streaming platforms such as [[entities/youtube]].

### Typical Toolchain
- **Mezzanine Export:** [[entities/prores]] or [[entities/dnxhr]] in a MOV container.
- **Delivery Encode:** [[entities/h264]] (High profile) or [[entities/hevc]] (Main10) using [[entities/adobe-media-encoder]] or [[entities/handbrake]].

### Benefits Highlighted in the Source Session
- Reduces the load on the editing machine during the first export.
- Allows the use of slower, higher‑quality encoder presets for the final file.
- Provides a clean archival master that can be reused for future delivery formats.

---
*Related concepts:* [[concepts/export-settings]], [[concepts/mezzanine-master]]

See also: [[summaries/session-31_2025-03-14]]