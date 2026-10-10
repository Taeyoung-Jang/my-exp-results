---
sources: ["summaries/session-08_2024-06-15.md"]
type: "Product"
description: "File History is Windows' built-in tool for continuous file-level backup to external drives."
---

## File History (Windows)

File History is the native Windows utility that continuously copies **personal files** (documents, photos, videos, etc.) to a designated external drive. It provides versioned, incremental backups, allowing you to restore previous versions of files easily.

### Key facts from [[summaries/session-08_2024-06-15]]
- Recommended as the primary **offline backup** method for Windows users alongside a cloud backup service [[concepts/cloud_backup]].
- Works well with an **encrypted external drive** that is plugged in roughly **once a month** to capture the latest changes.
- Complemented by occasional **full system images** using Windows’ built‑in "Backup and Restore (Windows 7)" tool or third‑party options like [[entities/macrium_reflect]] and [[entities/aomei_backupper]].
- Fits into a broader [[concepts/backup_strategy]]: primary local copy → automatic cloud copy → periodic offline copy.

### Typical workflow
1. Connect the encrypted external drive.
2. Enable File History to automatically back up designated libraries and folders.
3. Let the backup run (it’s incremental after the initial full copy).
4. Eject and store the drive safely until the next monthly run.

File History leverages the same **offline backup** principles discussed in the session, offering a low‑maintenance, cost‑effective solution for safeguarding personal data on Windows machines.