---
type: "Concept"
sources: ["summaries/session-32_2025-02-13.md", "summaries/session-12_2024-06-15.md"]
description: "A simple, rotating external‑drive method for automated local backups of user data."
---

# Local Backup Strategy

A **local backup strategy** is a lightweight, fully offline approach to protecting personal files. It relies on two or more external drives that rotate on a regular schedule, combined with built‑in OS tools to automate the copying of selected user folders.

## Core Elements

1. **Rotating Drives**
   - **Weekly drive**: Plug in once a week; runs an automatic backup of the chosen folders.
   - **Monthly drive**: Swapped in every month (or every few months) to create a second independent copy.
   - This redundancy protects against both accidental deletion and drive failure without using any cloud service.

2. **Targeted Folder Set**
   - Focus on personal data: `Documents`, `Pictures`, `Videos`, `Desktop`, and any custom `Projects` directory.
   - Avoid backing up the full system image; user folders are the irreplaceable assets.

3. **Automation Tool**
   - On **[[entities/windows_11]]**, the built‑in **[[entities/file_history]]** utility handles the scheduled copying.
   - Configure it to monitor the selected folders and to run whenever the external drive is connected.

4. **Backup Frequency & Retention**
   - Set the **backup frequency** to *daily* (or the smallest interval available). The tool will execute the backup the next time the drive is present, effectively giving you a weekly backup routine.
   - Use the **[[concepts/backup_retention_policy]]** "until space is needed" setting to let older versions be pruned automatically, keeping storage management simple.

## Benefits
- **No cloud dependency** – all data stays on physical media you control.
- **Low maintenance** – once the schedule and folders are defined, the process requires only weekly plug‑in.
- **Fast recovery** – restoring individual user files from File History is quick and granular.

## Relation to File Organization
A well‑structured folder hierarchy (see [[concepts/file_organization]]) complements this strategy by making the set of backed‑up items clear and consistent, reducing the chance of missed files.

## Example Implementation
The step‑by‑step instructions for enabling this on Windows 11 are documented in [[summaries/session-12_2024-06-15]], which walks through:
1. Connecting the drive and opening **Control Panel → System and Security → File History**.
2. Turning on File History and selecting the weekly drive.
3. Adding the custom `Projects` folder via **Advanced settings**.
4. Setting daily frequency and the "until space is needed" retention policy.

By following those steps, users can establish a reliable **local backup strategy** that balances simplicity, safety, and minimal ongoing effort.

See also: [[summaries/session-32_2025-02-13]]