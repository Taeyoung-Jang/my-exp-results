---
type: "Concept"
sources: ["summaries/session-37_2025-10-14.md", "summaries/session-11_2025-07-14.md"]
description: "A systematic approach for protecting data using layered local and off‑site copies, encryption, and appropriate tools."
---

# Backup Strategy

A **backup strategy** is a systematic approach to protecting digital data by maintaining multiple copies in different locations and formats. The goal is to guard against loss from hardware failure, accidental deletion, ransomware, or service outages.

## Core Elements (as described in [[summaries/session-11_2025-07-14]])

1. **Cloud backup** – Automatic, continuous syncing of files from laptops and phones to an online service. This provides an off‑site copy that is always up‑to‑date. [[concepts/cloud-backup]]
2. **External drive backup** – A physical storage device kept at home (or another safe location) that is connected periodically to create a second copy of all important data. This protects against cloud‑only failures and gives a tangible recovery option.
3. **System image backup** – A full‑disk snapshot (e.g., using "Backup and Restore (Windows 7)") stored on an external drive. It can restore the entire operating system, applications, and settings, including BitLocker and TPM state, to the exact pre‑failure state. [[concepts/system-image-backup]]
4. **Off‑site backup** – Storing irreplaceable personal files in a cloud drive or self‑hosted sync service (e.g., Syncthing) that is independent of the OS login. This adds a layer of redundancy beyond the local external drive. [[concepts/offsite-backup]]
5. **Encryption** – Securing any external or cloud‑based backup with strong encryption (e.g., BitLocker on Windows). This keeps data private if the media is lost or stolen. [[concepts/encryption]]
6. **Backup frequency** – For most users, connecting the external drive **once a month** is sufficient; power users may prefer a **weekly** schedule.
7. **Built‑in backup utilities** – Use the operating system’s native tools for automated, versioned backups:
   - **macOS**: [[entities/time-machine]] (or [[entities/filevault]] for full‑disk encryption). [[entities/macos]]
   - **Windows**: [[entities/file-history]] for personal‑file versioning, or the legacy **Backup and Restore (Windows 7)** for full system images. [[entities/windows]] [[entities/backup-and-restore-windows-7]]

## Why Combine Cloud and Local Backups?
- **Redundancy**: Two independent copies reduce the chance that a single failure wipes out data.
- **Version history**: Both cloud services and tools like Time Machine or File History keep older versions, allowing recovery of overwritten or accidentally deleted files.
- **Ease of use**: Cloud sync runs continuously without user intervention; the external drive backup runs on a simple, regular schedule.
- **Security**: Encrypting the external drive ensures that even if the physical media is compromised, the data remains protected.

## Practical Recommendations
- **Choose a reputable cloud provider** that offers automatic photo and document sync, or set up a self‑hosted sync using [[entities/syncthing]].
- **Purchase an external hard drive (SSD or HDD)** with enough capacity for at least one full backup of your important files.
- **Enable encryption** on the drive using the platform’s native solution (e.g., **BitLocker** on Windows). [[entities/bitlocker]]
- **Create a full system image** periodically with "Backup and Restore (Windows 7)" to guarantee rapid recovery of the entire OS.
- **Store the BitLocker recovery key** safely: save it to a USB drive, keep a copy in a secure note within your password manager, and optionally back it up off‑site.
- **Use a dedicated password manager** for cross‑device passwords and to keep recovery keys secure. Good options include [[entities/bitwarden]], [[entities/1password]], and [[entities/keepassxc]] (paired with a cloud folder or Syncthing). [[concepts/password-manager]]
- **Set a reminder** to connect the external drive monthly (or weekly for high‑change environments) and let the OS backup utility run.
- **Document your backup schedule and key locations** in a secure note within your password manager to ensure you can locate all copies quickly if disaster strikes.

By following this layered approach—combining cloud sync, external drive copies, full system images, encryption, and reliable password‑manager storage—everyday users can achieve a robust, low‑maintenance **backup strategy** that safeguards photos, documents, and other critical data with minimal hassle.

See also: [[summaries/session-37_2025-10-14]]