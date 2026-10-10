---
type: "Concept"
sources: ["summaries/session-32_2024-12-13.md"]
description: "Identifying and deleting redundant photos and videos during organization."
---

# Duplicate Removal

Duplicate removal is the process of locating and deleting redundant or unwanted media files—such as exact copies, near‑duplicates, or low‑quality shots—so that a photo archive remains lean, searchable, and easy to back up.

## Why it matters
- Reduces storage consumption on both the laptop and external backup drives.
- Speeds up cloud sync and local backup operations.
- Prevents clutter that can make trip‑folder navigation difficult.

## Typical workflow (as described in [[summaries/session-32_2024-12-13]])
1. **Incoming folder**: After each trip, dump all media into a single [[concepts/incoming-folder]] (e.g., "Photos Incoming").
2. **Quick pass**: Before moving files to a named trip folder, perform a rapid review to:
   - Delete obvious junk (accidental shots, blurry images).
   - Remove exact duplicates and near‑duplicates.
3. **Move to trip folder**: Once cleaned, place the remaining files into a consistently named folder following the [[concepts/trip-folder-naming]] convention (e.g., `2025-02 Japan`).
4. **Backup**: The cleaned archive is then protected by a [[concepts/cloud-backup]] service and mirrored to an external drive via a [[concepts/plug-and-forget-backup]] method such as [[entities/file-history]] on [[entities/windows]].

## Tools & techniques
- Manual visual inspection for obvious junk.
- Automated duplicate‑finder utilities (e.g., duplicate‑file scanners) can speed up the process, though the core idea is a **fast, repeatable pass** rather than a deep forensic review.
- Integrate duplicate removal into the overall [[concepts/backup-strategy]] to keep the workflow low‑effort.

## Related concepts
- [[concepts/incoming-folder]] – the staging area where duplicate removal begins.
- [[concepts/cloud-backup]] – ensures a remote copy exists after duplicates are cleared.
- [[concepts/external-drive-mirroring]] – keeps a local redundant copy after cleanup.
- [[concepts/plug-and-forget-backup]] – automates the sync of the cleaned archive.
- [[concepts/local-backup]] – the primary copy on the laptop that benefits from duplicate removal.
- [[concepts/trip-folder-naming]] – naming scheme that works best once duplicates are removed.
