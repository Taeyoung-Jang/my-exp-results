---
sources: ["summaries/session-01_2025-06-15.md"]
type: "Product"
description: "Apple ProRes is an Apple‑developed high‑quality intermediate video codec."
---

# Apple ProRes

Apple ProRes is a family of high‑performance, visually lossless video codecs developed by Apple for professional post‑production workflows. It is commonly used as a **mezzanine codec** because it preserves image quality while keeping file sizes manageable for editing and archiving.

## Key facts from [[summaries/session-01_2025-06-15]]
- Recommended as the preferred mezzanine format for macOS when exporting high‑resolution masters, such as 8K projects.
- Suggested profiles include **ProRes 422 HQ** for most workflows and **ProRes 4444** when alpha channel or higher color fidelity is required.
- Used in the described workflow as the export codec for both chunked intermediate files and the final stitched master, ensuring no generation loss.
- Paired with settings like 10‑bit depth, full resolution, and standard PCM audio (48 kHz, 24‑bit) in the example export presets.

## Related concepts and entities
- The role of ProRes as a [[concepts/mezzanine-codec]] is contrasted with delivery codecs such as H.264/H.265.
- In the recommended workflow, ProRes works alongside a [[concepts/proxy-workflow]] where low‑resolution proxies are edited before switching back to full‑resolution media for the final export.
- The chunked export approach described in the session references [[concepts/chunked-export]] and can be applied with ProRes as the intermediate format.
- Other tools and services mentioned for off‑loading renders include [[entities/adobe-team-projects]], [[entities/aws-ec2-g-series]], and [[entities/paperspace]].

## Typical usage scenarios
- Intermediate master files for high‑resolution (UHD, DCI, or anamorphic) projects.
- Archival copies where preserving color depth and detail is critical.
- Situations where downstream delivery requires a more compressed format; the ProRes master serves as a reliable source.

---
*For more context, see the full summary of the conversation in [[summaries/session-01_2025-06-15]].*