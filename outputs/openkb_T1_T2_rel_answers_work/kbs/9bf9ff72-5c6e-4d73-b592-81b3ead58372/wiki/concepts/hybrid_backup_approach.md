---
type: "Concept"
sources: ["summaries/session-33_2024-10-15.md"]
description: "Combines full-disk imaging with file‑level backups for flexibility and fast recovery."
---

## Hybrid Backup Approach

A **hybrid backup approach** blends two complementary backup methods: **full‑disk images** that capture the entire system state, and **file‑level backups** that copy specific folders and files. By using both, users get the safety net of a quick bare‑metal restore while retaining easy access to individual files for routine restores.

### Why use a hybrid approach?
- **Rapid full‑system recovery** – If the laptop fails, a disk image lets you restore the OS, applications, and settings in one step.
- **Simple file retrieval** – File‑level backups let you grab a single photo or document without mounting an image.
- **Redundancy of method** – If one backup type becomes corrupted, the other may still be usable.
- **Low‑stress automation** – When paired with [[concepts/auto_run_backup_software]], the hybrid workflow can run automatically each week, requiring minimal user interaction.

### Typical implementation (based on [[summaries/session-33_2024-10-15]])
| Platform | Tools | How it works |
|----------|-------|--------------|
| **Windows** | [[entities/macrium_reflect]] (or [[entities/easeus_todo_backup]]) | Configure the software to create a full system image **and** a separate file‑level job in the same session. Set the schedule to *run when the external drive is detected*.
| **macOS** | [[entities/time_machine]] (or [[entities/carbon_copy_cloner]]) | Time Machine already performs incremental file‑level backups; Carbon Copy Cloner can add a full‑disk clone that runs automatically when the drive is connected.

### Steps to set up
1. **Choose a cloud sync** service for continuous off‑site protection – see [[concepts/cloud_backup]].
2. **Connect an external drive** that stays unplugged most of the week ([[concepts/offline_backup]]).
3. **Install auto‑run backup software** (e.g., Macrium Reflect’s *run when disk becomes available* option) – see [[concepts/auto_run_backup_software]].
4. **Create two backup jobs**:
   - *Full disk image* – captures the entire system.
   - *File‑level copy* – backs up user folders such as Photos and Documents.
5. **Enable verification** after each run to ensure integrity.
6. **Schedule a quick restore test** every few months (see the restore checklist in the session summary).

### Benefits in context
The hybrid approach aligns with the broader [[concepts/low_stress_backup]] philosophy: a set‑and‑forget system that protects critical data while staying simple enough for weekly manual activation only. It also complements an overall [[concepts/backup_strategy]] that mixes cloud and offline copies for robust protection.

---
*This concept is derived from the recommendations in [[summaries/session-33_2024-10-15]].*