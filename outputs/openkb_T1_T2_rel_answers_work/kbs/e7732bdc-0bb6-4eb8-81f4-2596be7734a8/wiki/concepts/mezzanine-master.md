---
type: "Concept"
sources: ["summaries/session-07_2024-06-15.md"]
description: "A high‑quality intermediate file used before final delivery encoding."
---

# Mezzanine Master

A **mezzanine master** is a high‑quality, intermediate video file created as the first export step in a [[concepts/two-step-workflow]]. It preserves the original resolution, frame rate, and color fidelity while using a codec that is fast to render and easy on system resources. The mezzanine serves as the source for a later compression pass to the delivery format (e.g., YouTube).

---

## Core Characteristics
- **Purpose**: Decouple the demanding creative render from the intensive delivery encode, reducing crashes on modest hardware.
- **Typical Codecs**:
  - [[entities/prores]] (e.g., ProRes 422 or ProRes 422 HQ) on macOS
  - [[entities/dnxhr]] (e.g., DNxHR HQX) on Windows
- **Container**: Usually MOV (or MXF for DNxHR) to retain metadata and support high‑bit‑depth video.
- **Video Settings**:
  - Resolution and frame rate match the source timeline (e.g., 3840×2160 at 23.976 fps).
  - Bit depth: 10‑bit preferred for graded footage; 8‑bit if the source is 8‑bit.
  - Chroma subsampling: 4:2:2 to keep color detail for grading.
- **Audio Settings**: Uncompressed PCM, 48 kHz, 24‑bit.
- **Keyframe Interval**: Default/auto – not critical for mezzanine files.

---

## Relationship to Other Concepts
- **[[concepts/export-settings]]** – The mezzanine master is the first set of export settings in the overall pipeline. It prioritizes speed and lossless quality over file size.
- **[[concepts/two-step-workflow]]** – After creating the mezzanine, the second step uses a delivery codec (e.g., H.264, H.265) in a tool such as Adobe Media Encoder or HandBrake.

---

## Practical Checklist (from [[summaries/session-07_2024-06-15]])
### Archival Mezzanine – ProRes (macOS)
- **Container**: MOV
- **Codec**: ProRes 422 (or ProRes 422 HQ)
- **Resolution**: 3840×2160
- **Frame rate**: 23.976
- **Bit depth**: 10‑bit
- **Chroma**: 4:2:2
- **Audio**: PCM, 48 kHz, 24‑bit

### Archival Mezzanine – DNxHR (Windows)
- **Container**: MOV or MXF
- **Codec**: DNxHR HQX
- **Resolution**: 3840×2160
- **Frame rate**: 23.976
- **Bit depth**: 10‑bit
- **Chroma**: 4:2:2
- **Audio**: PCM, 48 kHz, 24‑bit

---

## Benefits
1. **Stability** – Rendering a lightweight codec reduces CPU/GPU load, preventing crashes.
2. **Flexibility** – The same mezzanine can be reused for multiple delivery targets (YouTube, broadcast, archival).
3. **Quality Preservation** – Lossless or visually lossless codecs keep grading, grain, and color grading intact for the final encode.

---

## When to Use
- Projects where the final delivery codec is computationally heavy (e.g., H.265, high‑bit‑rate H.264).
- Situations with limited hardware resources.
- Workflows requiring an archival‑grade master for future re‑encoding.
