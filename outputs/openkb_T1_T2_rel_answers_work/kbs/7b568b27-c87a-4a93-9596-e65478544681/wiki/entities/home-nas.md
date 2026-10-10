---
sources: ["summaries/session-11_2025-06-15.md"]
type: "Product"
description: "A locally hosted network‑attached storage device used for offline backups."
---

# Home NAS

**Type:** product

**Description:** A network‑attached storage (NAS) appliance kept at home, providing shared, always‑available storage for files and serving as an offline backup target.

## Role in the backup strategy
The *Home NAS* is recommended in the **two‑layer backup** approach described in [[summaries/session-11_2025-06-15]]. It functions as the **secondary** backup layer (Drive B) that stays disconnected from the primary computer most of the time, protecting against ransomware and simultaneous drive failures.

- **Primary layer (Drive A):** Automated, continuous backups using [[entities/file-history]] on the main computer.
- **Secondary layer (Drive B):** Either an external hard drive or a *Home NAS* that is plugged in weekly (or bi‑weekly) to receive a full system image or sync of the user data.

## Key characteristics
- **Offline protection:** By remaining unplugged, the NAS cannot be reached by malware that may encrypt or delete files on the primary drive.
- **Versioning support:** When combined with [[concepts/versioning]] from File History, the NAS stores periodic snapshots (e.g., weekly system images) that can be rolled back if needed.
- **Network accessibility:** Unlike a directly attached external drive, a NAS can be accessed from multiple devices on the home network, simplifying recovery across machines.

## Related concepts and entities
- [[concepts/two-layer-backup]] – the overall strategy that pairs continuous local backups with an offline copy.
- [[concepts/versioning]] – the mechanism that keeps multiple file versions, primarily handled by File History.
- [[concepts/local-file-organization]] – the broader context of keeping files in a simple, searchable structure.
- [[entities/external-drive]] – another possible choice for the secondary offline backup.
- [[entities/windows-11]] – operating system environment where the backup tools (File History, Windows Backup) run.
- [[entities/windows-backup-restore]] – the built‑in imaging tool used to create system images on the NAS.

## Summary reference
For the complete discussion of the backup plan that includes the *Home NAS*, see [[summaries/session-11_2025-06-15]].