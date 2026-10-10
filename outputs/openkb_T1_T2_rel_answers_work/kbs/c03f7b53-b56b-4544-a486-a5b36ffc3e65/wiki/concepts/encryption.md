---
type: "Concept"
sources: ["summaries/session-37_2025-10-14.md", "summaries/session-11_2025-07-14.md"]
description: "Encryption secures backup media with keys, enabling private offline copies alongside cloud storage."
---

# Encryption

Encryption protects data on storage media by requiring a password or recovery key to read the contents. In a personal [[concepts/backup-strategy]], encrypting an external drive adds a layer of security against loss or theft and ensures that only you can access the data.

## How it fits into backup

- **Cloud backup** stores copies online, but the provider often controls the encryption keys. Adding an encrypted local copy gives you exclusive control over the data.
- The external drive can be encrypted with macOS **FileVault** ([[entities/filevault]]) or Windows **BitLocker** ([[entities/bitlocker]]). Both integrate with the OS and require the same password/key on any machine that can unlock the drive.
- A full [[concepts/system-image-backup]] can be made of an encrypted drive. The image includes the BitLocker/TPM state and will restore cleanly on the same hardware, preserving encryption without additional steps.
- For off‑site copies, you may store an encrypted archive (e.g., a BitLocker‑protected VHD) in a [[concepts/offsite-backup]] service. The encryption remains under your control even when the files are in the cloud.

## Practical considerations from [[summaries/session-11_2025-07-14]] and session‑37

- Keep the encryption password or recovery key in a safe place; losing it makes recovery impossible.
- When using BitLocker on a local account, the recovery key is **not** automatically uploaded to a Microsoft profile. Manually save it to a USB drive **and** store a copy in a secure notes vault of a password manager such as **Bitwarden** ([[entities/bitwarden]]).
- Restoring a system image that includes BitLocker will usually boot without a prompt on the same machine. If you restore to different hardware or after a major firmware/TPM change, Windows will prompt for the recovery key.
- Encryption does not complicate restores as long as the key is available. Any compatible [[entities/windows]] or [[entities/windows-11]] device can unlock a BitLocker‑encrypted drive.

## Related concepts

- [[concepts/backup-strategy]]
- [[concepts/cloud-backup]]
- [[concepts/offsite-backup]]
- [[concepts/system-image-backup]]
- [[concepts/password-manager]]

See also: [[summaries/session-37_2025-10-14]]