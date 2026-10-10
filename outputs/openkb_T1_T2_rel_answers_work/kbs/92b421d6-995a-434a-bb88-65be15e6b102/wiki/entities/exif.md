---
sources: ["summaries/session-36_2024-12-15.md"]
type: "Other"
description: "Standard metadata format embedded in image files."
---

# EXIF (type: other)

**Description**: EXIF (Exchangeable Image File Format) is a widely used standard for storing metadata directly inside image files such as JPEG and PNG. It records details like capture date, camera settings, and location.

**Key points from [[summaries/session-36_2024-12-15]]**
- Recommended as the primary method for embedding metadata in photos for a future‑proof personal archive.
- Suggested to rely on embedded metadata rather than external indexes, because the data travels with the file across devices and backup systems.
- Paired with XMP (see [[entities/xmp]]) when richer or custom metadata is needed.

**Related concepts**
- [[concepts/open-formats]] – using open, well‑supported file formats (e.g., JPEG, PNG) ensures EXIF data remains readable in the long term.
- [[concepts/backup-strategy]] – embedded EXIF survives backup and restore processes without requiring additional metadata files.

**Related entities**
- [[entities/jpeg]] – a common image format that natively supports EXIF.
- [[entities/png]] – also supports EXIF, though less frequently used for photography.

**Practical usage**
- Store photos in folders organized by year (see [[concepts/folder-structure]]) with filenames like `YYYY-MM-DD‑keyword.ext` while retaining EXIF data for chronological context.
- When creating or editing images, preserve the original EXIF block; avoid stripping it unless privacy concerns dictate.
