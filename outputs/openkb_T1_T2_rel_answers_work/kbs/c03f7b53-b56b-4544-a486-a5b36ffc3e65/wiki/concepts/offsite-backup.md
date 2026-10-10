---
type: "Concept"
sources: ["summaries/session-37_2025-10-14.md"]
description: "Offsite backup stores copies of critical data to a remote location for disaster recovery."
---

# Offsite Backup

Offsite backup refers to the practice of copying important files and data to a storage location that is physically separate from the primary device. By keeping a redundant copy outside the local environment, users protect themselves against hardware failure, theft, ransomware, or other localized disasters.

## Why Use Offsite Backup?
- **Disaster resilience** – If the laptop is lost, damaged, or its internal storage fails, the offsite copy remains accessible.
- **Protection against ransomware** – An encrypted local drive cannot encrypt the remote backup if it is stored in a separate service.
- **Device‑agnostic access** – Files can be retrieved from any internet‑connected machine without needing the original device.

## Recommendations from [[summaries/session-37_2025-10-14]]
In the session‑37 discussion (Windows 11, local‑only account), the following practical steps were suggested for an offsite backup strategy:

1. **Identify irreplaceable data** – documents, photos, work files, and any other personal information that cannot be recreated.
2. **Choose a cloud‑drive service or self‑hosted sync** – examples include a standard cloud storage account (e.g., OneDrive, Google Drive) used solely for specific folders, or a self‑hosted solution like [[entities/syncthing]] that syncs a designated folder to a home server.
3. **Configure selective folder sync** – only the folders containing the identified irreplaceable data should be synced, keeping the rest purely local.
4. **Secure the transmission** – ensure the chosen service encrypts data in transit (HTTPS/TLS) and, if possible, at rest. This ties into the broader [[concepts/encryption]] concept.
5. **Maintain a separate backup schedule** – offsite backups should be updated regularly (daily or weekly) independent of the local [[concepts/system-image-backup]] routine.

## Relationship to Other Backup Concepts
- **[[concepts/backup-strategy]]** – Offsite backup is a core component of a comprehensive backup strategy, complementing local backups such as system images or File History.
- **[[concepts/cloud-backup]]** – When the offsite destination is a commercial cloud storage provider, the practice aligns with cloud‑backup principles, though the focus remains on selective, user‑controlled syncing rather than a full account‑wide backup.
- **[[concepts/system-image-backup]]** – System images protect the entire operating system state locally; offsite backup protects the user’s most valuable data in a remote location.

## Practical Tips
- **Use strong, unique passwords** for the cloud account and store them in a reputable [[concepts/password-manager]] (e.g., [[entities/bitwarden]], [[entities/1password]], or [[entities/keepassxc]]).
- **Enable two‑factor authentication** on the cloud service to prevent unauthorized access.
- **Periodically verify** that the offsite copies are complete and restorable.
- **Consider encryption at rest** if the provider does not encrypt by default; you can encrypt the files locally before syncing.

By integrating offsite backup as outlined, users with a local‑only Windows account can maintain privacy and stability while still enjoying a reliable safety net for their most critical data.
