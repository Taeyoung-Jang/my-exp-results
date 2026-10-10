---
sources: ["summaries/session-11_2025-06-15.md"]
type: "Product"
description: "Legacy Windows tool for creating system image backups"
---

## Windows Backup and Restore (Windows 7)

**What it is**
- A built‑in Windows utility (carried over from Windows 7) that creates full system image backups and can also back up selected files. It is accessible in Windows 11 via the *Control Panel* under *Backup and Restore (Windows 7)*.

**Key facts from [[summaries/session-11_2025-06-15]]**
- Recommended as the **primary backup method for Drive A** in the two‑layer backup strategy, complementing continuous versioning from [[entities/file-history]].
- Used to produce a **boot‑recoverable system image** on an external drive, providing a restore point if the OS fails to start.
- Paired with a secondary offline drive (often a [[entities/external-drive]] or a [[entities/home-nas]]) for the **secondary backup layer**.

**Role in the backup plan**
- Supplies **full‑disk snapshots** that protect against drive failure, corruption, or ransomware that might affect the live system.
- Works together with the versioning capabilities of [[entities/file-history]] to give both granular file‑level recovery and whole‑system restore.

**Related concepts**
- Part of the broader [[concepts/two-layer-backup]] approach.
- Relies on the idea of **[[concepts/versioning]]** for file‑level safety, while providing a separate offline image for disaster recovery.

**Compatibility**
- Fully supported on [[entities/windows-11]]; runs without additional installation.

---
*This page aggregates information from the session‑11 discussion and links to related concepts and entities within the knowledge base.*