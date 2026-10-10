---
sources: ["summaries/session-07_2024-06-15.md"]
type: "Product"
description: "Avid DNxHR is a high‑quality intermediate codec for 4K video mastering."
---

# Avid DNxHR

Avid DNxHR (Digital Nonlinear Extensible High‑Resolution) is a professional‑grade intermediate **video codec** designed for high‑resolution workflows, especially 4K UHD editing and export.

## Key Facts from [[summaries/session-07_2024-06-15]]
- **Intended role**: Used as a *mezzanine master* in a **two‑step workflow** to create a stable, visually lossless intermediate file before final delivery. [[concepts/mezzanine-master]] [[concepts/two-step-workflow]]
- **Recommended variant**: **DNxHR HQX**, which provides 10‑bit color depth and 4:2:2 chroma subsampling for demanding color‑graded projects.
- **Resolution & frame rate**: 3840×2160 (4K UHD) at 23.976 fps, matching the source timeline.
- **Audio handling**: Uncompressed PCM, 48 kHz, 24‑bit.
- **Container options**: Typically exported in **MOV** or **MXF** containers.
- **Performance benefit**: Faster, less crash‑prone rendering on modest hardware compared to direct H.264/H.265 encoding.

## Relation to Other Concepts & Entities
- It is one of the primary choices for **export‑settings** when prioritizing quality and stability. [[concepts/export-settings]]
- Often contrasted with **Apple ProRes** for cross‑platform workflows. [[entities/prores]]
- After the mezzanine export, the file is commonly handed to an encoder such as **HandBrake** or **Adobe Media Encoder** for final H.264/H.265 delivery. [[entities/handbrake]] [[entities/adobe-media-encoder]]
- The final delivery formats may target platforms like **YouTube**. [[entities/youtube]]

## Usage Summary
1. **Export** your 4K timeline to a DNxHR HQX mezzanine master using the settings listed above.
2. **Feed** the resulting .mov/.mxf file into a dedicated encoder (e.g., HandBrake) to produce a compressed delivery (H.264 or H.265). 
3. **Benefit**: The heavy lifting of decoding and color processing stays in the first pass, while the second pass focuses solely on bitrate compression, reducing crashes on limited hardware.

---
*This page aggregates the practical guidance for Avid DNxHR as presented in the session‑07 discussion.*