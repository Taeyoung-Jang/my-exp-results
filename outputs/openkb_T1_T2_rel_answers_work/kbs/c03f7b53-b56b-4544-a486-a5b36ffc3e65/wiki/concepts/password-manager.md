---
type: "Concept"
sources: ["summaries/session-37_2025-10-14.md"]
description: "A tool that stores and syncs passwords securely, independent of the OS login."
---

# Password Manager

A **password manager** is a secure vault that stores login credentials, generates strong passwords, and can synchronize them across devices without relying on the operating system's native account system.

## Why Use a Standalone Manager?
- **Privacy**: Credentials stay under your control; no need to link a Microsoft or Apple account to the OS. 
- **Security**: Most managers encrypt the vault locally with a master password and use zero‑knowledge encryption, meaning the service provider cannot read your data. See [[concepts/encryption]].
- **Cross‑platform convenience**: Access your passwords on Windows, macOS, Linux, Android, or iOS without granting the OS full identity access.

## Recommendations from [[summaries/session-37_2025-10-14]]
The session suggests three practical options for Windows 11 users who keep a local account:
- **Bitwarden** – a cloud‑based vault that offers free sync and strong open‑source security. [[entities/bitwarden]]
- **1Password** – a premium service with polished UI and robust team features. [[entities/1password]]
- **KeePassXC** paired with a sync layer (e.g., a cloud folder or Syncthing) for a self‑hosted solution. [[entities/keepassxc]] [[entities/syncthing]]

All three operate **outside** the Windows credential store, so they do not “take over” the login process.

## How It Fits Into a Backup Strategy
While a password manager protects credentials, you still need to back up the vault file itself. Treat the vault as an **off‑site backup** asset: store an encrypted copy in a cloud drive or on an external drive. This aligns with the broader [[concepts/offsite-backup]] approach discussed in the session.

## Integration with System Security Features
- **BitLocker** and TPM protect the disk, but the recovery key must be saved manually when using a local account. The password manager vault can be a convenient place to store that key securely. [[entities/bitlocker]] [[entities/tpm]]
- A local Windows 11 account combined with a standalone manager gives you a stable, privacy‑focused environment while still enjoying the convenience of synchronized passwords.

---
*Related concepts*: [[concepts/encryption]], [[concepts/offsite-backup]], [[concepts/cloud-backup]], [[concepts/backup-strategy]]