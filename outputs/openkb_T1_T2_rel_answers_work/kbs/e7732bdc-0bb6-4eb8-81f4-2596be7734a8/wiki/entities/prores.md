---
sources: ["summaries/session-07_2024-06-15.md"]
type: "Product"
description: "Apple ProRes is a high‑quality intermediate video codec for editing and archiving."
---

# Apple ProRes

Apple ProRes is a family of high‑quality intermediate codecs designed for professional video editing and archiving. It provides visually lossless compression, fast decode/encode performance, and is widely supported in macOS‑based workflows.

## Key facts from [[summaries/session-07_2024-06-15]]
- **Recommended role**: Used as the primary [[concepts/mezzanine-master]] format for 4K UHD exports.
- **Performance**: Offers fast, reliable renders with minimal CPU/GPU load, making it ideal for machines that struggle with heavy encoding.
- **Typical settings**:
  - Container: **MOV** (or MXF for some workflows)
  - Resolution: 3840×2160 (4K UHD)
  - Frame rate: 23.976 fps (as per source timeline)
  - Bit depth: 10‑bit (preserves grading and grain)
  - Chroma subsampling: 4:2:2
  - Audio: PCM, 48 kHz, 24‑bit
- **Workflow integration**: Forms the first step in a [[concepts/two-step-workflow]], where the mezzanine master is later compressed to delivery formats such as H.264 or HEVC.
- **Export settings guidance**: Aligns with [[concepts/export-settings]] best practices—matching source resolution and frame rate, avoiding unnecessary scaling or sharpening.

## Related entities and tools
- [[entities/dnxhr]] – Alternative mezzanine codec for Windows environments.
- [[entities/h264]] – Common delivery codec for YouTube uploads.
- [[entities/hevc]] – Also known as H.265, recommended for efficient delivery.
- [[entities/adobe-media-encoder]] – Popular encoder for the second‑pass compression step.
- [[entities/handbrake]] – Free tool that can encode the mezzanine master to H.264/H.265.
- [[entities/youtube]] – Target platform for the final delivery version.

## Usage notes
- **Why choose ProRes**: It balances high visual fidelity with low processing overhead, reducing the risk of crashes during the initial export.
- **When to prefer DNxHR**: On Windows systems where ProRes support is limited, DNxHR HQX serves a similar purpose.
- **Final delivery**: After creating the ProRes mezzanine, the project is typically re‑encoded to H.264 or HEVC for streaming platforms, following the two‑step workflow.
