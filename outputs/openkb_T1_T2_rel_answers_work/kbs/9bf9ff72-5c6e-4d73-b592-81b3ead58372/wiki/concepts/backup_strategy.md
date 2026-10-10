---
type: "Concept"
sources: ["summaries/session-33_2024-10-15.md", "summaries/session-08_2024-06-15.md"]
description: "A systematic plan combining cloud sync, auto‑run offline backups, and verification to protect data."
---

# Backup Strategy

A **backup strategy** is a systematic plan for protecting digital data by creating redundant copies in different locations using appropriate tools. It aims to balance convenience, cost, and security while ensuring data can be restored after loss events. The overall approach is a [[concepts/low_stress_backup]] that requires minimal user interaction.

## Core Layers
1. **Primary layer** – The active computer where files are created and edited daily.
2. **Automatic cloud layer** – Continuous, versioned backup to a reputable cloud service. This provides hands‑off, off‑site protection and easy access from any device. [[concepts/cloud_backup]]
3. **Offline layer** – A periodic, encrypted backup to a physical external drive stored separately from the primary machine. This defends against cloud‑service outages, ransomware, and accidental deletions. [[concepts/offline_backup]]

## Frequency & Redundancy
- **Typical cadence**: Plug the external drive and run a full backup once a month (or every 6–8 weeks for low activity). For a weekly routine, use auto‑run software to start the backup as soon as the drive is connected. [[concepts/auto_run_backup_software]]
- **Redundancy**: One encrypted drive is sufficient when paired with cloud backup; a second drive or off‑site rotation adds extra peace of mind but is optional.
- **Versioning**: Cloud services retain historic versions, while the offline drive keeps a clean snapshot.

## Security Practices
- Enable **encryption** on both cloud storage and the external drive.
- Use **strong passwords** and **two‑factor authentication** for cloud accounts.
- Store the offline drive in a safe location (e.g., a lock‑able drawer) when not in use.

## Recommended Tools
- **macOS** – [[entities/time_machine]] for automated, versioned file backups to the external drive. Carbon Copy Cloner can also auto‑run when the target disk appears. [[entities/carbon_copy_cloner]]
- **Windows** – [[entities/file_history]] for personal files, complemented by occasional full system images using [[entities/macrium_reflect]] or [[entities/easeus_todo_backup]] (or [[entities/aomei_backupper]]). Both can be configured to start automatically when the drive is connected. [[concepts/auto_run_backup_software]]
- **Hybrid approach** – Combine full‑disk imaging with file‑level backups to get fast bare‑metal recovery and easy file retrieval. [[concepts/hybrid_backup_approach]]

## Restore Testing
- Perform a quick restore check every few months: restore 1‑2 recent files and verify they open.
- Conduct a deeper test once or twice a year: browse a backup image or verify the full system restore process.

## Benefits of the Strategy
- **Convenient**: Daily work stays local; cloud sync runs automatically; offline backups start with no manual steps.
- **Cost‑effective**: Only one modest external drive plus existing cloud subscription.
- **Secure**: Encryption and off‑site redundancy protect against hardware failure, malware, and physical disasters.

## Related Concepts
- [[concepts/cloud_backup]]
- [[concepts/offline_backup]]
- [[concepts/low_stress_backup]]
- [[concepts/auto_run_backup_software]]
- [[concepts/hybrid_backup_approach]]

---
**Source summary**: [[summaries/session-08_2024-06-15]] and [[summaries/session-33_2024-10-15]]