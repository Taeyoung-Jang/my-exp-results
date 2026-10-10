---
sources: ["summaries/session-37_2025-10-14.md", "summaries/session-11_2025-07-14.md"]
type: "Product"
description: "Windows built-in tool that version‑backs personal files."
---

# File History

**Type**: product

File History is a built‑in backup feature of [[entities/windows]] that continuously copies changed files from user libraries, desktop, contacts, and favorites to a designated external drive or network location. It provides versioned snapshots, allowing users to restore previous versions of documents, photos, and other personal data.

## Key Points from [[summaries/session-11_2025-07-14]]
- Recommended as the primary **[[concepts/backup-strategy]]** for personal files on Windows when paired with cloud storage.
- Considered sufficient for most users who mainly need to protect photos and documents.
- Suggested as an alternative to a full **[[entities/backup-and-restore-windows-7]]** system image when ease of use is a priority.
- Works well alongside an **encrypted external drive** (see [[concepts/encryption]]). Encryption of the backup drive does not complicate restores as long as the password or recovery key is kept safe.

## Related Concepts and Entities
- [[concepts/backup-strategy]] – overall approach combining cloud and local backups.
- [[concepts/cloud-backup]] – the cloud component that syncs files automatically.
- [[concepts/encryption]] – recommended for securing the external drive used by File History.
- [[entities/backup-and-restore-windows-7]] – alternative Windows built‑in tool for full system images.
- [[entities/bitlocker]] – Windows encryption technology often used to protect the external drive that stores File History backups.

## Usage Guidance
1. **Enable File History** via Settings → Update & Security → Backup.
2. Choose a reliable external drive or network share as the backup destination.
3. Keep the drive **encrypted** (e.g., with [[entities/bitlocker]]) and retain the recovery key.
4. For additional protection, keep a cloud sync service active for the same files.

File History provides a low‑maintenance, versioned backup solution that fits the 3‑2‑1 backup model when paired with cloud storage and an encrypted external drive.

See also: [[summaries/session-37_2025-10-14]]