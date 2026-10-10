---
sources: ["summaries/session-36_2024-12-15.md"]
type: "Other"
description: "XMP is a standard for embedding metadata in digital files."
---

# XMP (Extensible Metadata Platform)

**Type:** other

**Description:** XMP (Extensible Metadata Platform) is a widely‑adopted, open standard for storing metadata directly inside digital files such as images, PDFs, and other media formats.

## Key Facts from [[summaries/session-36_2024-12-15]]
- Recommended as the preferred method for embedding metadata in photos and other assets, alongside EXIF (see [[entities/exif]]) and front‑matter for Markdown files.
- Supports rich, structured data (author, rights, keywords, timestamps) that travels with the file when it is moved across devices, storage media, or backup services.
- Encouraged in the **future‑proof archive** workflow to avoid reliance on external databases.

## Relationships
- Part of the broader **open‑formats** strategy discussed in [[concepts/open-formats]].
- Works hand‑in‑hand with file‑level organization concepts such as [[concepts/folder-structure]] and backup planning [[concepts/backup-strategy]].
- Complementary to other metadata standards like EXIF (image‑specific) and front‑matter in Markdown files (see [[entities/markdown]]).

## Usage Recommendations (from the session)
1. **Embed metadata** in images (JPEG, PNG) using XMP to ensure information persists across copies.
2. For text‑based notes, store similar context in Markdown front‑matter while using XMP for any attached images.
3. Verify integrity of embedded metadata during backup cycles, leveraging checksums as part of the backup strategy.

---
*This entity page captures XMP’s role as described in the session‑36 discussion on building resilient personal archives.*