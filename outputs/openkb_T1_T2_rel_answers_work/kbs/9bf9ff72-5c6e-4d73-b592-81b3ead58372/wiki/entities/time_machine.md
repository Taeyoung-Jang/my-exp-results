---
sources: ["summaries/session-33_2024-10-15.md"]
type: "Product"
description: "Time Machine is macOS’s built‑in backup product that runs automatically when a drive is connected."
---

# Time Machine

**Type:** Product

Time Machine is the native backup utility included with macOS. It automatically detects an attached external drive and begins incremental backups without user intervention, making it a classic example of a [[concepts/low_stress_backup]] and [[concepts/auto_run_backup_software]] solution.

### Key points from [[summaries/session-33_2024-10-15]]
- Works perfectly with a **weekly offline backup** routine: keep the drive unplugged during the week and plug it in on Sundays; Time Machine will catch up immediately.
- Provides continuous, versioned copies of user folders, which satisfies the [[concepts/cloud_backup]] principle of off‑site redundancy when paired with a cloud sync service.
- Can be combined with a [[concepts/hybrid_backup_approach]]: use Time Machine for daily file‑level backups and a separate imaging tool (e.g., [[entities/macrium_reflect]]) for occasional full‑system images.
- Requires no manual scheduling; the backup starts as soon as the drive appears, reducing the risk of missed backups – a core benefit of [[concepts/offline_backup]] strategies.

### Related tools and alternatives
- **Carbon Copy Cloner** – a third‑party macOS backup app that also offers auto‑run capabilities and can create bootable clones. See [[entities/carbon_copy_cloner]].
- **EaseUS ToDo Backup** – mentioned for Windows users; not directly comparable but part of the broader backup ecosystem. See [[entities/easeus_todo_backup]].

### Why it matters
Time Machine’s simplicity and integration with macOS make it an ideal component of a [[concepts/backup_strategy]] that aims for minimal maintenance while still delivering reliable protection for photos, documents, and system files.