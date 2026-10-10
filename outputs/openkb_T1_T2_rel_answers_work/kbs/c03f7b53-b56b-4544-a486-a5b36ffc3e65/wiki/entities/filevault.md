---
sources: ["summaries/session-11_2025-07-14.md"]
type: "Product"
description: "Apple's built‑in macOS disk encryption tool for protecting data."
---

# FileVault

**Type:** product

## Overview
FileVault is the native full‑disk encryption feature of **[[entities/macos]]**. It encrypts the entire startup drive (or any external drive) using XTS‑AES‑128 encryption, protecting data at rest from theft or loss.

## Role in a Backup Strategy
In the backup approach discussed in [[summaries/session-11_2025-07-14]], FileVault is recommended for securing the external drive that complements cloud storage. By encrypting the drive, users add a layer of [[concepts/encryption]] that guards against unauthorized access if the drive is misplaced.

## How It Works
- When enabled, FileVault encrypts the drive automatically; the user provides a password or recovery key.
- The same encrypted drive can be unlocked on any Mac that knows the password or key, so restores are not tied to a specific computer.
- Encryption does **not** impede regular backup tools like **[[entities/time-machine]]**; Time Machine can back up to a FileVault‑protected drive.

## Comparison to Windows Alternatives
- The Windows counterpart is **[[entities/bitlocker]]**, which offers similar full‑disk encryption.
- For external drives on Windows, File History or **[[entities/backup-and-restore-windows-7]]** can be used, but encryption should still be applied via BitLocker.

## Key Takeaways
- Use FileVault to encrypt external backups for robust [[concepts/backup-strategy]].
- Keep the password or recovery key stored safely; loss of the key is the only barrier to restore.
- Pair with cloud backup (see [[concepts/cloud-backup]]) for a comprehensive 3‑2‑1 protection model.