---
sources: ["summaries/session-05_2024-06-15.md"]
type: "Product"
description: "Open‑source media server for streaming personal collections."
---

# Jellyfin (product)

Jellyfin is a free, open‑source media server that lets users organize, stream, and access their personal video and audio libraries across devices such as TVs, phones, and tablets. In the context of **session‑05_2024‑06‑15**, Jellyfin is recommended as one of the primary software options for serving a ripped Blu‑ray and CD collection at home.

## Key Facts from the Session
- **Purpose**: Provides a self‑hosted alternative to commercial streaming services, enabling private streaming of ripped media without subscription fees.
- **Compatibility**: Works on low‑power hardware like an [[entities/intel_nuc]] or a NAS, and can be paired with external Blu‑ray drives for disc ripping.
- **Workflow Integration**:
  - Media is ripped using tools such as [[entities/makemkv]] (for Blu‑rays) and [[entities/handbrake]] (for encoding).
  - The resulting files are stored on the media server and indexed by Jellyfin for easy browsing.
- **Advantages**:
  - Maintains true ownership of media, aligning with the [[concepts/convenience_vs_ownership]] discussion.
  - Supports DRM‑free digital files, complementing the [[concepts/drm_free_downloads]] approach.
- **Alternative**: The commercial counterpart [[entities/plex]] is also mentioned, but Jellyfin offers a cost‑free solution.

## Related Concepts
- [[concepts/disc_ripping]] – the process of extracting media from physical discs before serving it via Jellyfin.
- [[concepts/convenience_vs_ownership]] – Jellyfin helps balance convenience with true ownership.
- [[concepts/drm_free_downloads]] – works well with DRM‑free files obtained from sources like Bandcamp.

## Reference
- Summarized in [[summaries/session-05_2024-06-15]].