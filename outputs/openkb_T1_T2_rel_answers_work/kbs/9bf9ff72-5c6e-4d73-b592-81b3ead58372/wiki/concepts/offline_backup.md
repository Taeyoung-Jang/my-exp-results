---
type: "Concept"
sources: ["summaries/session-33_2024-10-15.md", "summaries/session-08_2024-06-15.md"]
description: "Offline backup stores encrypted copies of data on a physically separate, non‑online device for resilient protection."
---

# Offline Backup

**Definition**: Offline backup is a periodic, encrypted copy of your data stored on a physically separate device that is not continuously connected to the internet or your primary computer.

## Why it matters
- Provides protection against ransomware, cloud‑account lockouts, and accidental online deletions.
- Complements [[concepts/cloud_backup]] to satisfy the classic 3‑2‑1 backup rule (3 copies, 2 media types, 1 off‑site).

## Core recommendations from [[summaries/session-08_2024-06-15]]
- **Device**: A single external hard drive is the most cost‑effective choice for most users; a NAS is optional for multi‑device environments.
- **Encryption**: Encrypt the drive (e.g., using BitLocker or macOS FileVault) before storing any backups.
- **Frequency**: Plug in and run a full backup **once a month** (or every 6‑8 weeks if file changes are minimal). More frequent runs are useful for high‑activity periods.
- **Location**: Keeping the drive at home is sufficient for many; off‑site rotation (friend’s house, safe deposit box) adds fire‑theft protection but isn’t mandatory.
- **Redundancy**: One drive meets the 3‑2‑1 goal when paired with cloud backup; a second drive is a peace‑of‑mind upgrade for long‑term archival.

## Additional guidance from [[summaries/session-33_2024-10-15]]
- **Low‑stress design**: Treat the offline backup as a [[concepts/low_stress_backup]] component that runs automatically with minimal user interaction.
- **Auto‑run backup software**: Choose tools that start the job as soon as the drive is connected – e.g., [[entities/macrium_reflect]] or [[entities/easeus_todo_backup]] on Windows, and Time Machine or [[entities/carbon_copy_cloner]] on macOS. This aligns with the [[concepts/auto_run_backup_software]] principle.
- **Hybrid backup approach**: Combine a full system image with a file‑level copy in the same session – a [[concepts/hybrid_backup_approach]] that gives both quick bare‑metal recovery and easy file retrieval.
- **Verification**: Enable the software’s post‑run verification so you know the backup is intact.
- **Restore testing**: Perform a quick restore check every couple of months (restore 1‑2 recent files and open them) and a deeper test once or twice a year (mount an image, browse, verify critical folders). This keeps you confident the backup isn’t silently broken.
- **Secondary off‑site copy**: Keep a small cloud sync copy (photos, irreplaceable docs) as an additional safety net, without making it a primary backup.

## Workflow summary
1. **Connect** the encrypted external drive.
2. Run the platform‑specific backup tool (auto‑started):
   - macOS → Time Machine (file/folder backups) or Carbon Copy Cloner (full image).
   - Windows → Macrium Reflect or EaseUS ToDo Backup for a full image, plus File History for file‑level copies.
3. **Verify** the backup completed successfully (enable verification).
4. **Eject** the drive and store it safely.
5. **Test restores** on the schedule described above.

## Related concepts
- [[concepts/backup_strategy]] – overall plan that includes both cloud and offline layers.
- [[concepts/cloud_backup]] – the always‑online component that works alongside offline backup.
- backup frequency – how often backups should run.
- encryption – securing both cloud and offline copies.

---
*This page synthesises practical guidance from the session‑08 discussion and the later session‑33 update, presenting offline backup as a simple, low‑cost, and secure layer in a robust data‑protection strategy.*