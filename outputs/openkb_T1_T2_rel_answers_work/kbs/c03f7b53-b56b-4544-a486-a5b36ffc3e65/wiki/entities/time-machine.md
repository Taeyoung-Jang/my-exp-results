---
sources: ["summaries/session-11_2025-07-14.md"]
type: "Product"
description: "macOS built‑in backup utility that creates automatic, versioned copies of files."
---

# Time Machine

Time Machine is the backup solution bundled with **macOS**. It automatically copies files from your Mac to an attached external drive, preserving version history and allowing easy restoration of individual items or the entire system.

## Key Points from [[summaries/session-11_2025-07-14]]
- Recommended as the **local backup** component of a simple [[concepts/backup-strategy]] that pairs cloud storage with an encrypted external drive.
- Works seamlessly when the drive is connected on a **monthly** (or weekly) schedule, providing an offline copy in case of cloud sync errors or account issues.
- Supports **encryption** of the external drive; restoring files only requires the password or recovery key, not the original Mac.
- Offers versioned backups, making it easier to recover accidentally deleted or overwritten files.

## Related Concepts and Entities
- [[concepts/backup-strategy]] – the overall approach of combining cloud and local backups.
- [[concepts/encryption]] – securing the external drive used with Time Machine.
- [[entities/macos]] – the operating system that includes Time Machine.
- [[concepts/cloud-backup]] – the complementary cloud storage layer mentioned alongside Time Machine.
