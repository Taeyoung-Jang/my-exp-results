---
type: "Concept"
sources: ["summaries/session-05_2024-06-15.md"]
description: "Extracting audio/video from physical discs to digital files for personal use."
---

# Disc Ripping

**Definition**: The process of converting media stored on physical discs (Blu‑rays, DVDs, CDs) into digital files that can be stored, backed up, and streamed locally.

## Why Disc Ripping?
- Provides **digital convenience** while retaining true ownership of the original media, addressing the trade‑off highlighted in [[summaries/session-05_2024-06-15]].
- Enables streaming‑like access across devices without relying on subscription services, linking to the broader theme of [[concepts/convenience_vs_ownership]].

## Typical Workflow (as described in the source session)
1. **Hardware**: A low‑power computer such as an [[entities/intel_nuc]] or a NAS, paired with an external Blu‑ray drive.
2. **Ripping Software**:
   - Use **MakeMKV** ([[entities/makemkv]]) to extract the raw video from Blu‑rays.
   - Encode or re‑package with **HandBrake** ([[entities/handbrake]]) for size‑efficient formats.
3. **Audio Extraction**: Standard CD‑ripping tools (not listed in the whitelist) can be used for music.
4. **Media Server**: Store the resulting files on the machine and serve them via **Plex** ([[entities/plex]]) or **Jellyfin** ([[entities/jellyfin]]) for playback on TVs, phones, and tablets.

## Legal & Ethical Considerations
- Ripping should be limited to media you own and for **personal, non‑commercial** use, respecting local copyright law.
- The practice aligns with the concept of **DRM‑free** ownership; however, only DRM‑free purchases (see [[concepts/drm_free_downloads]]) guarantee that the resulting files remain fully usable.

## Backup Strategy
- Keep the master library on the primary device (NUC/NAS).
- Mirror the library to at least one external hard drive, rotating backups periodically.
- Store a second backup in a separate location within the home to protect against hardware failure.
- Regularly verify integrity and migrate to newer storage media to avoid bit‑rot.

## Benefits Summary
- **Ownership**: Digital copies remain under your control, unlike streaming licenses.
- **Convenience**: Files can be streamed locally via a media server.
- **Longevity**: With proper backups, the digital library can outlast the physical discs.

---
*Related concepts*: [[concepts/convenience_vs_ownership]], [[concepts/drm_free_downloads]]
*Source*: [[summaries/session-05_2024-06-15]]