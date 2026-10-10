---
type: "Concept"
sources: ["summaries/session-32_2025-09-12.md", "summaries/session-15_2025-06-15.md"]
description: "A strategy for reliable, offline data protection using multiple local backups."
---

# Offline Backup Strategy

**Definition** – An offline backup strategy is a set of practices that keep copies of important data on local, non‑cloud storage devices to ensure reliability, privacy, and redundancy without relying on internet services.

## Core Principles
- **Reliability** – Backups must run automatically and be easy to verify. See [[concepts/backup-reliability]].
- **Redundancy** – Store at least two separate copies in physically distinct locations to protect against hardware failure or disasters. See [[concepts/backup-redundancy]].
- **Privacy** – Use full‑disk encryption on external drives to keep data confidential.

## Recommended Architecture (from [[summaries/session-15_2025-06-15]])
1. **Primary device** – Your computer or phone holds the live data.
2. **Backup Drive A** – Permanently connected to the primary device for continuous, automatic backups.
3. **Backup Drive B** – Connected only occasionally and stored in a different location (e.g., another room or a safe) to provide physical separation.

This “two‑drive + primary device” model satisfies both reliability and redundancy while staying completely offline.

## Encryption Approach
- Prefer **full‑disk encryption** of each external drive for simplicity; a single password protects all files.
- Per‑category encrypted containers are optional and add friction unless you need separate passwords.

## Operational Practices
- **Regular imports** – For phone photos, use a USB connection (or [[entities/mtp]] on Android) to import images into a consistent folder hierarchy on the computer.
- **Note exports** – Ensure note‑taking apps store plain files; otherwise export notes weekly.
- **Restore testing** – Perform a quick restore check every 2–3 months by retrieving a few files from each backup device.

## Optional Enhancements
- A **NAS** can serve as a central backup hub if you want always‑on local network storage, but it introduces additional maintenance.
- Encrypted disk images can replace full‑disk encryption if you prefer container‑based security.

## Summary Checklist
- [ ] Set up two external drives with automatic backup software.
- [ ] Enable full‑disk encryption on both drives.
- [ ] Schedule weekly photo imports via [[entities/usb]] (or [[entities/mtp]] for Android).
- [ ] Export notes from proprietary apps on a weekly basis.
- [ ] Test restores every two months.

By following these steps, users achieve a robust offline backup strategy that maximizes data safety without any cloud dependency.

See also: [[summaries/session-32_2025-09-12]]