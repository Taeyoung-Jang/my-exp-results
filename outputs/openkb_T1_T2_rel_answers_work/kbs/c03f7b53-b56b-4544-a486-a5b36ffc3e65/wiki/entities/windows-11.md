---
sources: ["summaries/session-37_2025-10-14.md"]
type: "Product"
description: "Microsoft's 2021‑released Windows 11 operating system for PCs."
---

# Windows 11

Windows 11 is the latest major release of Microsoft’s desktop operating system, succeeding Windows 10. It introduces a refreshed UI, updated system requirements, and tighter integration with cloud services while retaining compatibility with a wide range of hardware.

## Relevance in [[summaries/session-37_2025-10-14]]
The session discusses using **Windows 11** with a **local user account** to prioritize privacy and stability. The advice recommends keeping the core login local and adding selective cloud features for backups, password sync, and recovery.

## Backup strategy for Windows 11
- **Full system image**: Use the built‑in "Backup and Restore (Windows 7)" tool (see [[entities/backup-and-restore-windows-7]]) to create periodic system images. This aligns with the [[concepts/system-image-backup]] approach recommended in the session.
- **Off‑site file backup**: Store personal documents in a cloud drive or self‑hosted sync solution (e.g., [[entities/syncthing]]) following the [[concepts/offsite-backup]] model.
- **File History**: Optional versioned backup for selected folders, linked to [[entities/file-history]].

## Security and encryption
- **BitLocker**: Windows 11 supports device‑level encryption via BitLocker. When using a local account, the recovery key must be saved manually (see [[entities/bitlocker]] and [[entities/tpm]]). This ties into the broader [[concepts/encryption]] discussion.
- **TPM**: Trusted Platform Module hardware works with BitLocker to protect keys; users must manage recovery keys themselves.

## Password management without a Microsoft account
The session recommends standalone password managers that operate independently of Windows login:
- [[entities/bitwarden]]
- [[entities/1password]]
- [[entities/keepassxc]] (can be paired with a cloud folder for sync)
These tools embody the [[concepts/password-manager]] concept and avoid the automatic credential sync of a [[entities/microsoft-account]].

## Related concepts and entities
- [[concepts/backup-strategy]] – overall approach to protecting data on Windows 11.
- [[concepts/cloud-backup]] – optional cloud storage for selected folders.
- [[entities/windows]] – the broader Windows family.
- [[entities/macos]] and [[entities/filevault]] – mentioned for comparison of native encryption solutions.
- [[entities/time-machine]] – macOS counterpart to Windows backup tools.

---
*This page synthesizes the key points about Windows 11 from the session‑37 discussion, linking to relevant concepts and related entities.*