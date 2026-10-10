---
sources: ["summaries/session-37_2025-10-14.md"]
type: "Product"
description: "KeePassXC is an open‑source password manager that stores vaults locally and syncs via user‑chosen cloud services."
---

# KeePassXC

KeePassXC is a cross‑platform, open‑source password manager that stores encrypted password vaults locally on the device. Users can sync the vault file through any cloud service or self‑hosted sync tool, giving full control over where the data resides.

## Key facts from Session 37 (2025‑10‑14)
- Recommended as a **local‑account‑friendly** password manager that does **not** integrate with the Windows login system, preserving privacy and stability. [[summaries/session-37_2025-10-14]]
- Can be paired with a cloud‑synced folder (e.g., via **Syncthing**) to achieve cross‑device password availability without tying to a Microsoft account. [[entities/syncthing]]
- Serves as an alternative to cloud‑centric managers like **Bitwarden** and **1Password**, fitting the **password‑manager** concept for users who want self‑hosted control. [[entities/bitwarden]] [[entities/1password]] [[concepts/password-manager]]

## How it fits into a backup strategy
- The vault file can be included in **off‑site backup** routines, ensuring recovery even if the local machine fails. [[concepts/offsite-backup]]
- Because the vault is a regular file, it can be protected by **BitLocker** encryption for the whole disk, complementing the overall **encryption** approach. [[entities/bitlocker]] [[concepts/encryption]]
- It works well alongside **system‑image‑backup** for full‑system restores, as the vault is part of the captured image. [[concepts/system-image-backup]]

## Typical usage pattern
1. Create a master password and generate a local vault file.
2. Store the vault in a folder that is synced via a chosen cloud service (e.g., OneDrive, Dropbox, Syncthing).
3. Optionally enable **File History** for versioned copies of the vault folder, though the primary protection comes from the encrypted vault itself. [[entities/file-history]]

## Related entities and concepts
- **Windows 11**: KeePassXC runs on Windows 11 and does not require a Microsoft account. [[entities/windows-11]]
- **TPM**: When used on a device with BitLocker, the TPM stores the encryption keys, while KeePassXC manages the password vault separately. [[entities/tpm]]
- **Backup and Restore (Windows 7)**: The system‑image backup method can capture KeePassXC vaults alongside the OS. [[entities/backup-and-restore-windows-7]]

---
*KeePassXC offers a privacy‑preserving, flexible password management solution that aligns with a local‑account‑first Windows setup.*