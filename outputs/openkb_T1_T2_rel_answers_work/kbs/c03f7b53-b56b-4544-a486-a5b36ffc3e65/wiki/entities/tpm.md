---
sources: ["summaries/session-37_2025-10-14.md"]
type: "Other"
description: "Hardware security chip that stores cryptographic keys for Windows encryption."
---

# TPM (Trusted Platform Module)

The TPM is a dedicated microcontroller built into most modern PCs that provides **hardware‑based security**. It stores cryptographic keys, measurements, and other secrets used by the operating system to protect data and ensure platform integrity.

## Role in Windows 11
- Windows 11 leverages the TPM for features like **BitLocker** drive encryption and secure boot. The TPM securely holds the BitLocker keys, making it harder for attackers to extract them.
- When using a **local Windows account**, BitLocker does **not** automatically upload the recovery key to a Microsoft account; you must back it up yourself (e.g., to a USB drive or a password manager). This was highlighted in [[summaries/session-37_2025-10-14]] where the need to manually save the recovery key was emphasized.

## Interaction with Backup & Recovery
- Restoring a **system image** (see [[concepts/system-image-backup]]) on the same hardware usually restores the TPM‑protected state without prompting for a recovery key. However, if the hardware changes (different motherboard, TPM version, or firmware update), Windows will prompt for the BitLocker recovery key because the TPM no longer matches the stored measurements.
- As part of a **backup‑strategy**, ensure the BitLocker recovery key is stored in a safe off‑site location (e.g., an encrypted note in a password manager like [[entities/bitwarden]] or on an external USB drive).

## Security Benefits
- Provides **encryption key isolation**: keys never leave the TPM unencrypted, protecting them from malware that compromises the OS.
- Supports **measured boot**: each boot component is measured and recorded, helping detect tampering.

## Practical Recommendations (from session‑37)
1. Keep the TPM enabled in BIOS/UEFI.
2. Use BitLocker for full‑disk encryption and back up the recovery key manually.
3. Pair BitLocker with a reliable **system image backup** to simplify recovery.
4. Store the recovery key in a secure location that is separate from the device (e.g., a password manager or an encrypted external drive).

---
*Related concepts*: [[concepts/encryption]], [[concepts/backup-strategy]]
*Related entities*: [[entities/bitlocker]], [[entities/windows-11]], [[entities/windows]]