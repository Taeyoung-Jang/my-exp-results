---
sources: ["summaries/session-01_2025-06-15.md"]
type: "Product"
description: "DNxHR is Avid's high‑quality intermediate codec for video editing."
---

# Avid DNxHR (product)

Avid DNxHR (Digital Nonlinear Extensible High Resolution) is a family of high‑performance, visually lossless intermediate codecs designed for editing and mastering high‑resolution video, especially 8K and beyond. It is the Windows‑centric counterpart to Apple ProRes and is widely used in professional workflows that require efficient encoding while preserving image fidelity.

## Key facts from [[summaries/session-01_2025-06-15]]
- **Recommended for Windows Premiere Pro users** when exporting 8K master and chunk files.
- **Codec profiles** mentioned: **DNxHR HQ** for standard 10‑bit workflows and **DNxHR HQX** for higher‑bit‑depth log footage.
- **Container**: typically exported in a QuickTime MOV wrapper (can also be MXF for delivery).
- **Settings**: 10‑bit depth, full 8K resolution, PCM audio 48 kHz 24‑bit, with “Render at Maximum Depth” and “Use Maximum Render Quality” usually turned off to keep render times reasonable.
- **Workflow role**: Serves as the **[[concepts/mezzanine-codec]]** in the advised chunked export and final master process, providing a balance between quality, file size, and render performance.

## Related concepts and entities
- [[concepts/chunked-export]] – the workflow of splitting an 8K project into 5‑10‑minute segments and exporting each with DNxHR.
- [[concepts/mezzanine-codec]] – DNxHR is used as the mezzanine codec in the recommended pipeline.
- [[concepts/proxy-workflow]] – proxies are suggested for editing before the final DNxHR export.
- [[entities/adobe-premiere-pro]] – the editing application where DNxHR settings are applied.
- [[entities/adobe-team-projects]] – a possible off‑loading destination for DNxHR renders.
- [[entities/aws-ec2-g-series]] and [[entities/paperspace]] – cloud platforms where DNxHR exports can be rendered remotely.