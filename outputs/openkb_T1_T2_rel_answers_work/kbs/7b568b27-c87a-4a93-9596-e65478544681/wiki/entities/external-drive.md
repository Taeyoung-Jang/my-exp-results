---
sources: ["summaries/session-11_2025-06-15.md"]
type: "Product"
description: "Portable storage device used as primary and secondary backup in a local file system."
---

# External Drive

An **External Drive** is a portable storage product that serves as the backbone of the **two‑layer backup** strategy described in [[summaries/session-11_2025-06-15]].

## Role in the backup plan
- **Drive A** (primary): kept continuously connected to the computer and used by [[entities/file-history]] on [[entities/windows-11]] to provide continuous [[concepts/versioning]] of user files.
- **Drive B** (secondary/offline): plugged in on a weekly or bi‑weekly schedule to store a full system image using [[entities/windows-backup-restore]], acting as an offline safeguard against ransomware and drive failure.

## Interaction with file organization
The drive works with a simple [[concepts/local-file-organization]] layout – a handful of top‑level folders (Documents, Media, Projects, Inbox, System). By storing the entire user folder hierarchy on the external drive, the backup process captures the structure without requiring complex taxonomy.

## Key benefits
- **Redundancy**: Two independent physical copies protect against hardware loss.
- **Versioning**: Continuous snapshots via File History let you revert accidental deletions or unwanted changes.
- **Low maintenance**: Once configured, the drive requires only periodic plugging of the secondary device.

---
*Related pages*: [[concepts/two-layer-backup]], [[concepts/versioning]], [[entities/windows-11]], [[entities/windows-backup-restore]]