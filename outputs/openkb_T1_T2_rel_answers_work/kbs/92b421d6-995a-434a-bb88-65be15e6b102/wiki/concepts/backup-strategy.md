---
type: "Concept"
sources: ["summaries/session-36_2024-12-15.md"]
description: "A resilient 3‑2‑1 backup plan with versioning and integrity checks for personal archives."
---

# Backup Strategy

A **backup strategy** outlines how to protect personal digital archives against loss, corruption, or obsolescence. The approach advocated in [[summaries/session-36_2024-12-15]] follows a simplified **3‑2‑1 rule**:

1. **Primary archive** stored on the main computer.
2. **Local mirror** on a separate external drive.
3. **Off‑site/cloud backup** that retains historical versions.

### Key Elements

- **Versioning**: The cloud service should keep past versions of files so you can roll back after accidental edits or deletions.
- **Integrity verification**: Enable checksums or other integrity checks if the backup platform supports them; this catches silent corruption.
- **Automation**: Schedule regular syncs (e.g., daily or weekly) so backups happen without manual intervention.
- **Restore testing**: Periodically perform a test restore to verify that the backup data is usable.

### Relationship to Other Concepts

- The backup plan assumes a clear **[[concepts/folder-structure]]** (year‑based top‑level categories and a stable `Projects/` hierarchy) so that the same directory layout can be mirrored across storage locations.
- Using **[[concepts/open-formats]]** (Markdown, JPEG/PNG, MP4, PDF/A, etc.) ensures that backed‑up files remain accessible even if specific applications disappear.

### Practical Tips

- Store the backup configuration in a simple text or Markdown file within the archive root for easy reference.
- Keep at least two independent cloud providers if possible, adding an extra layer of geographic redundancy.
- For very large media collections, consider incremental backups to reduce bandwidth and storage costs.

By adhering to these guidelines, a personal archive can remain safe and recoverable for decades, even as hardware and software ecosystems evolve.
