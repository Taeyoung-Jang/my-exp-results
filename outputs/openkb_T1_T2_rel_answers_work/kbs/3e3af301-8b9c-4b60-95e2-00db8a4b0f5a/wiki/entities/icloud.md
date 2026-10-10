---
sources: ["summaries/session-37_2024-12-01.md"]
type: "Product"
description: "Apple iCloud is Apple’s cloud storage and sync service for devices."
---

## Apple iCloud (product)

Apple iCloud is Apple’s cloud‑based storage and synchronization platform that lets users back up data, sync files, photos, emails, contacts, and app settings across macOS, iOS, and other Apple devices.

### Role in session‑37_2024‑12‑01
The session discusses iCloud as one of the key cloud‑sync services to verify after a fresh‑start reinstall. It emphasizes:
- Checking that **iCloud Drive** and **iCloud Photos** show fully uploaded content before wiping the machine.
- Using the iCloud web UI to confirm completeness rather than trusting a local cache, which helps avoid re‑introducing stale or junk files.
- Recognizing that notes stored in iCloud are generally safe, but any locally‑only 2FA recovery codes or license files saved outside iCloud must be backed up separately.

### Practical considerations
- **Verification**: Open the iCloud website or the iCloud settings panel on a clean system and review the file list, recent activity, and any sync errors.
- **Backup checklist**: iCloud appears in the broader [[concepts/backup-checklist]] for cloud‑sync services that need validation during a fresh start.
- **Data safety**: Since iCloud automatically syncs many app data (e.g., Notes, Photos), it reduces the need for manual export, but users should still confirm that no local‑only items (like SSH keys or 2FA codes) are stored only on the device.

### Related entities & concepts
- Related product: [[entities/macos]] (the OS that tightly integrates with iCloud).
- Related concepts: [[concepts/fresh-start-decision]], [[concepts/backup-checklist]], [[concepts/data-migration-safety]].

### Source
This information is drawn from [[summaries/session-37_2024-12-01]].