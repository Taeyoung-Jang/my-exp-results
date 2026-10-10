---
sources: ["summaries/session-37_2025-10-14.md", "summaries/session-11_2025-07-14.md"]
type: "Product"
description: "BitLocker is Windows' built‑in drive encryption product."
---

# BitLocker

**Type:** Product

BitLocker is a built‑in encryption feature of **[[entities/windows]]** that allows users to protect the data on internal or external drives with strong encryption. In the context of the backup strategy discussed in [[summaries/session-11_2025-07-14]], BitLocker is recommended for securing an external backup drive.

## Key Points from the Session
- **Purpose:** Provides offline protection for a backup drive, preventing data access if the drive is lost or stolen.
- **Compatibility:** Integrated with Windows; can encrypt both internal system disks and removable drives.
- **Recovery:** Requires a password or recovery key; keeping this key safe is essential for successful restores.
- **Impact on Restores:** Encryption does **not** complicate restoring files as long as the recovery key is available. The drive can be unlocked on any Windows machine.
- **Relation to Backup Strategy:** Complements a **[[concepts/backup-strategy]]** that combines cloud storage with an encrypted external drive.

## Related Concepts and Entities
- [[concepts/encryption]] – the broader principle of protecting data through cryptographic methods.
- [[entities/file-history]] – another Windows backup tool mentioned alongside BitLocker for versioned file backups.
- [[entities/backup-and-restore-windows-7]] – an alternative Windows built‑in tool for creating full system images, which may be used in addition to BitLocker depending on user needs.
- [[concepts/backup-strategy]] – the overall approach of using both cloud and local encrypted backups.

---

*This page aggregates the information about BitLocker as presented in the conversation summary [[summaries/session-11_2025-07-14]].*

See also: [[summaries/session-37_2025-10-14]]