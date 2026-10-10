---
sources: ["summaries/session-37_2025-10-14.md", "summaries/session-11_2025-07-14.md"]
type: "Product"
description: "Legacy Windows utility for creating system images and file backups."
---

# Backup and Restore (Windows 7)

**Type:** product

**Overview**

Backup and Restore (Windows 7) is a built‑in Windows utility that allows users to create full system image backups and restore them to the same or a new machine. It is part of a broader [[concepts/backup-strategy]] for Windows users who want an offline, versioned copy of their data.

**Key Features**
- Creates complete system‑image files that capture the operating system, installed programs, settings, and user data.
- Supports scheduled backups to an external drive.
- Can be used in conjunction with cloud services for a layered backup approach.
- Works alongside but separately from the newer [[entities/file-history]] feature, which focuses on personal‑file versioning.

**Relation to Encryption**

While the tool itself does not encrypt backups, users are encouraged to store the backup drive on an encrypted volume (e.g., using [[entities/bitlocker]] on Windows) to protect the data, aligning with best practices around [[concepts/encryption]].

**Use Cases Mentioned in Session 11**
- Offered as an alternative to File History when a full system image is desired.
- Recommended for users who want a reliable offline copy in addition to cloud backups.

**Platform**
- Available on [[entities/windows]] operating systems, primarily Windows 7 and later versions that retain the utility.

**Cross‑Reference**
- See the discussion of backup recommendations in [[summaries/session-11_2025-07-14]], which contrasts this tool with other options like [[entities/file-history]] and cloud backup.


See also: [[summaries/session-37_2025-10-14]]