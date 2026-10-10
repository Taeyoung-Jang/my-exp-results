---
sources: ["summaries/session-36_2024-12-15.md"]
type: "Other"
description: "A widely used lossy image format recommended for long‑term archival."
---

# JPEG

**Type:** other

JPEG (Joint Photographic Experts Group) is a ubiquitous raster image format that uses lossy compression to achieve small file sizes while preserving acceptable visual quality. In the context of personal archiving, it is highlighted in [[summaries/session-36_2024-12-15]] as one of the **open, widely supported formats** suitable for future‑proof storage.

## Why JPEG is recommended
- **Broad compatibility:** Almost every device, operating system, and image viewer can read JPEG, ensuring accessibility decades from now.
- **Embedded metadata support:** JPEG files can store EXIF and XMP data directly within the file, which aligns with the recommended practice of **embedding metadata** rather than relying on external indexes. See related entities [[entities/exif]] and [[entities/xmp]].
- **Efficient storage:** The compression reduces storage requirements, making it easier to maintain multiple backups as suggested in the [[concepts/backup-strategy]] guidelines.

## Recommended usage in an archive
1. Store original, high‑quality JPEGs in the `Photos/` hierarchy defined by the [[concepts/folder-structure]] (e.g., `Photos/2026/2026‑03‑Trip‑to‑Japan`).
2. Use clear, chronological filenames such as `YYYY‑MM‑DD‑keyword‑description.jpg` to keep files sortable and self‑describing.
3. Ensure EXIF/XMP fields are populated with capture date, location, and any relevant tags to preserve context without external databases.
4. Include a brief `README.md` at the project or folder root to explain any collection‑wide conventions, keeping the README concise as advised in the session summary.

## Limitations
- Being lossy, JPEG is not ideal for archival of raw image data where every pixel matters; for such cases, lossless formats like PNG may be preferred (see [[entities/png]]). However, for everyday photos and documents where storage efficiency is a priority, JPEG remains a pragmatic choice.

---
*This entity page draws its key points from the recommendations in [[summaries/session-36_2024-12-15]] regarding long‑term personal archiving.*