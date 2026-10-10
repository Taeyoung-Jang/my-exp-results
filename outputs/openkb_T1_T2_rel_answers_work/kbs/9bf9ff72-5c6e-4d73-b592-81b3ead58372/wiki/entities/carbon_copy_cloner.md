---
sources: ["summaries/session-33_2024-10-15.md"]
type: "Product"
description: "macOS backup utility that auto‑runs when a drive is connected"
---

# Carbon Copy Cloner

**Type:** Product  

Carbon Copy Cloner (CCC) is a macOS backup utility that can automatically run backup jobs when a target disk is connected. It was recommended in [[summaries/session-33_2024-10-15]] as an alternative to Time Machine for users who want a low‑maintenance, auto‑run solution.

## Key facts from the session
- Works with the “plug‑in‑and‑run” workflow described in [[concepts/low_stress_backup]].
- Can be configured to start backups automatically when the external drive appears, fulfilling [[concepts/auto_run_backup_software]] requirements.
- Supports both full‑disk imaging and file‑level backups, fitting a [[concepts/hybrid_backup_approach]].
- Provides a browsable backup image, allowing quick verification of contents.

## Related concepts
- [[concepts/low_stress_backup]]
- [[concepts/auto_run_backup_software]]
- [[concepts/hybrid_backup_approach]]

## Related entities
- [[entities/time_machine]] (built‑in macOS backup tool)
- [[entities/macrium_reflect]] (Windows counterpart mentioned in the same session)

## Usage scenario
In the recommended weekly offline backup strategy, users keep an external drive unplugged and plug it in on Sundays. CCC can detect the drive, launch the predefined backup job, and verify the backup without further user interaction, reducing the risk of missed backups.