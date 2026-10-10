---
type: "Concept"
sources: ["summaries/session-37_2025-10-14.md"]
description: "A full‑machine snapshot stored externally that enables complete OS recovery."
---

# System Image Backup

**Type:** Concept

**Description:** A full‑machine snapshot stored on an external medium that can restore the entire Windows installation, applications, settings, and encrypted state.

---

## Definition
A *system image backup* captures the complete state of a computer’s system drive—including the operating system, installed programs, user settings, and any disk encryption metadata—into a single image file. Restoring this image returns the machine to the exact point in time when the backup was taken.

## Why Use It?
- **Full recovery**: Unlike file‑level backups, a system image can bring a non‑booting PC back to a working state.
- **BitLocker & TPM continuity**: When restored on the same hardware, the BitLocker encryption and TPM keys are preserved, avoiding immediate recovery‑key prompts.
- **Stability for non‑technical users**: Provides a “one‑click” restore path without needing to reinstall applications or reconfigure settings.

## Core Components (as described in [[summaries/session-37_2025-10-14]])
- **Tool**: Windows built‑in *Backup and Restore (Windows 7)* utility (`[[entities/backup-and-restore-windows-7]]`).
- **Target OS**: [[entities/windows-11]] (or other Windows versions).
- **Storage**: External USB drive or network share that is *off‑site* for disaster protection (`[[concepts/offsite-backup]]`).
- **Encryption considerations**: If BitLocker (`[[entities/bitlocker]]`) protects the system drive, the recovery key must be saved separately (e.g., USB, password manager) because a local account does not auto‑upload the key to a Microsoft profile.

## How It Fits Into a Backup Strategy
System image backup is a cornerstone of the overall [[concepts/backup-strategy]]. It complements:
- **File‑level versioning** (`[[entities/file-history]]`) for everyday file changes.
- **Off‑site cloud copies** (`[[concepts/cloud-backup]]` or `[[concepts/offsite-backup]]`) for critical documents.
- **Encryption** (`[[concepts/encryption]]`) to keep the image data protected when stored off‑site.

## Implementation Steps (derived from session‑37 guidance)
1. **Prepare an external drive** – format it with NTFS and ensure enough capacity for a full system image.
2. **Launch Backup and Restore (Windows 7)** – select *Create a system image* and point to the external drive.
3. **Include BitLocker recovery key** – manually export the key (`[[entities/bitlocker]]` → *Manage BitLocker*) and store it securely (e.g., in a password manager like `[[entities/bitwarden]]` or `[[entities/keepassxc]]`).
4. **Schedule regular images** – monthly or after major system changes.
5. **Test a restore** – boot from a Windows recovery drive and verify the image restores without prompting for a new BitLocker key (hardware unchanged).
6. **Combine with off‑site backups** – copy the image file to a secure cloud location or secondary external drive for true disaster resilience.

## Gotchas
- Restoring to **different hardware** (new motherboard, different TPM) will trigger a BitLocker recovery‑key prompt.
- Ensure the recovery key is stored *outside* the encrypted system image; otherwise you could be locked out.
- System images can be large; monitor storage limits on the external medium.

---

**Related concepts**: [[concepts/backup-strategy]], [[concepts/cloud-backup]], [[concepts/encryption]], [[concepts/offsite-backup]], [[concepts/password-manager]]
