---
type: "Concept"
sources: ["summaries/session-33_2025-08-15.md", "summaries/session-01_2025-06-15.md"]
description: "High-quality intermediate format for archiving and processing before final delivery"
---

# Mezzanine Codec

A mezzanine codec is a high‑quality, intermediate video format used for archiving or further processing before final delivery. It balances visual fidelity with manageable file sizes and render times, making it ideal for workflows that involve proxy editing, chunked exports, or cloud rendering.

## Why Use a Mezzanine Codec
- **Visually lossless**: Preserves the original image quality while keeping compression low enough to avoid massive files.
- **Edit‑friendly**: Works well with proxy workflows ([[concepts/proxy-workflow]]) and chunked export strategies ([[concepts/chunked-export]]) because it can be re‑wrapped without re-encoding.
- **Hardware‑aware**: Supports hardware acceleration on many platforms, reducing render time compared to raw or heavily compressed delivery formats.

## Common Mezzanine Codecs
| Platform | Codec | Typical Container | Bit Depth | When to Choose |
|----------|-------|-------------------|----------|----------------|
| macOS | **Apple ProRes 422 HQ** / **ProRes 4444** | MOV | 10‑bit | High‑color‑depth projects, extensive grading |
| Windows | **Avid DNxHR HQ** (or HQX for 10‑bit log) | MOV (or MXF) | 10‑bit | 8K or high‑resolution masters, cross‑platform exchange |

The source document [[summaries/session-01_2025-06-15]] recommends ProRes 422 HQ on macOS and DNxHR HQ on Windows as the default mezzanine choices for an 8K Premiere Pro workflow.

## Workflow Integration
1. **Edit with proxies** – Work on low‑resolution proxy files, keeping the full‑resolution media linked beneath.
2. **Export chunks** – Render 5–10 minute segments using the same mezzanine codec; this avoids generation loss.
3. **Stitch & final master** – Re‑wrap the chunks into a single file using the identical mezzanine preset, preserving quality.
4. **Off‑load if needed** – Transfer the project to a stronger workstation via [[entities/adobe-team-projects]] or rent a cloud VM such as [[entities/aws-ec2-g-series]] or [[entities/paperspace]] for the final export.

## Choosing Between ProRes and DNxHR
- Use **Apple ProRes** when working primarily on macOS or when the workflow requires 10‑bit color and alpha channels.
- Use **Avid DNxHR** on Windows or cross‑platform pipelines; HQ offers a good balance, while HQX provides extra headroom for log footage.

---

*Related concepts*: [[concepts/chunked-export]], [[concepts/proxy-workflow]].

See also: [[summaries/session-33_2025-08-15]]