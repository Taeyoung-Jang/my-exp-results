---
sources: ["summaries/session-11_2025-07-14.md"]
type: "Product"
description: "Microsoft's PC operating system, referenced in backup guidance."
---

# Windows

Windows is Microsoft’s flagship operating system for personal computers. In the **session-11_2025-07-14** discussion, Windows was referenced when comparing backup options for everyday users.

## Backup Context from the Session
- The conversation highlighted the need for a solid [[concepts/backup-strategy]] that pairs cloud storage with an encrypted external drive.
- For Windows, the built‑in options mentioned were **File History** and the legacy **Backup and Restore (Windows 7)** utility. These are linked as [[entities/file-history]] and [[entities/backup-and-restore-windows-7]].
- Encryption of the external drive can be performed with **BitLocker**, which is the Windows counterpart to macOS FileVault. See [[entities/bitlocker]] for details.

## Key Points
1. **File History** provides versioned backups of personal folders and is sufficient for most users who primarily need to protect photos and documents.
2. **Backup and Restore (Windows 7)** offers full‑system image capabilities for those who want to restore the entire OS state.
3. Encrypting the external drive with BitLocker enhances security without complicating restores, as long as the recovery key or password is stored safely.

## Related Concepts and Entities
- [[concepts/cloud-backup]] – the cloud component of the recommended strategy.
- [[concepts/encryption]] – why encrypting the external drive matters.
- [[entities/filevault]] – macOS equivalent of BitLocker, mentioned for cross‑platform comparison.
- [[entities/macos]] – another platform discussed alongside Windows.
- [[entities/time-machine]] – macOS native backup tool, contrasted with Windows options.

## Reference Summary
For a concise overview of the advice given, see the session summary: [[summaries/session-11_2025-07-14]].