---
type: "Concept"
sources: ["summaries/session-33_2024-10-15.md"]
description: "Backup tools that start automatically when the target drive is detected."
---

# Auto‑Run Backup Software

**Definition**: Software that initiates a backup job automatically as soon as the designated backup drive becomes available, eliminating manual start‑up steps.

## Why it matters
In a low‑stress backup strategy, the goal is to make the backup process *hands‑free* so it isn’t forgotten.  The session‑33_2024-10-15 discussion emphasizes that the biggest source of failure is human inertia – “plug it in and it runs.”  By using an auto‑run solution the user only has to remember to connect the external drive on a scheduled day (e.g., Sunday); the software takes care of the rest, including verification of the backup.

## Key characteristics
- **Drive‑detect trigger** – The program monitors USB/Thunderbolt connections and launches the predefined job instantly when the target disk appears.
- **Pre‑configured job** – Backup sets, schedules, and verification options are defined once and then run without further user input.
- **Verification step** – Most auto‑run tools provide a post‑backup integrity check, satisfying the best‑practice recommendation to verify backups each run.
- **Cross‑platform options** – Windows examples include [[entities/macrium_reflect]] and [[entities/easeus_todo_backup]]; macOS users can rely on the built‑in [[entities/time_machine]] which already auto‑starts when the Time Machine drive connects.

## Recommended tools (from the source)
| Platform | Tool | Auto‑run capability |
|----------|------|----------------------|
| Windows  | Macrium Reflect Home | Detects drive, runs scheduled image/folder job automatically |
| Windows  | EaseUS ToDo Backup | Same auto‑run behavior when the drive is detected |
| macOS    | Time Machine | Built‑in auto‑run when the backup disk is mounted |
| macOS    | Carbon Copy Cloner | Can be set to auto‑run on disk appearance (mentioned as an option) |

## How it fits into broader concepts
- Part of a [[concepts/low_stress_backup]] design, reducing manual steps.
- Works together with a [[concepts/cloud_backup]] for off‑site redundancy.
- Often implemented in a [[concepts/hybrid_backup_approach]] where both full‑disk images and file‑level copies are created in the same auto‑run session.
- Complements an [[concepts/offline_backup]] routine where the external drive sits unplugged most of the week.

## Practical checklist for setting up auto‑run backup software
1. **Select a tool** that supports “run when drive becomes available.”
2. **Create the backup job** – choose full image, file‑level, or both.
3. **Enable verification** – checksum or integrity check after each run.
4. **Test the trigger** – unplug the drive, reconnect, and confirm the job starts without prompts.
5. **Document the setup** – note the schedule, job type, and verification method in a simple reference (e.g., a text file on the desktop).

## Reference
- This concept is directly discussed in [[summaries/session-33_2024-10-15]], which recommends auto‑run tools for a weekly offline‑drive backup routine.
