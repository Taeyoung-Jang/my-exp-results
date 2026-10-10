---
type: "Concept"
sources: ["summaries/session-37_2025-10-14.md", "summaries/session-11_2025-07-14.md"]
description: "Storing data on remote servers to add off‑site redundancy and easy device access."
---

## Cloud Backup

Cloud backup refers to the practice of storing copies of files, photos, and documents on remote servers operated by a cloud service provider. It offers automatic synchronization across devices, ensuring that data is continuously protected without user intervention.

### Why Use Cloud Backup?
- **Always‑on protection** – Files are uploaded in real time from laptops, phones, and tablets.
- **Off‑site safety** – Data is stored away from local hardware failures, theft, or natural disasters.
- **Device independence** – Access your files from any internet‑connected device.
- **Versioning** – Many services keep historical versions, allowing recovery from accidental changes.
- **Selective sync without OS‑level account linkage** – You can use a cloud‑driven folder or app independently of a Windows or Microsoft account, giving you the safety‑net of off‑site copies while keeping your local Windows login strictly local (as recommended in [[summaries/session-37_2025-10-14]]).

### Role in a Comprehensive Backup Strategy
Cloud backup is a core component of a [[concepts/backup-strategy]] that also includes a local, encrypted external drive and periodic system images. While the cloud provides convenience and redundancy, the external drive protects against cloud‑specific failures such as accidental deletions, sync errors, or account issues. Combining cloud backup (off‑site) with a full [[concepts/system-image-backup]] on an external drive gives both quick recovery of individual files and a reliable path to restore an entire system.

### Interaction with Encryption
Although cloud services often encrypt data in transit and at rest, users may still wish to encrypt files before uploading for additional privacy. This concept ties into [[concepts/encryption]], which covers encrypting local backups (e.g., using [[entities/bitlocker]] on Windows or [[entities/filevault]] on macOS). Encrypting files prior to cloud upload ensures that only you hold the keys, even if the service provider’s encryption is compromised.

### Reference
For a practical discussion of cloud backup within a simple personal backup plan, see the summary of [[summaries/session-11_2025-07-14]].