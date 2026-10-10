---
type: "Concept"
sources: ["summaries/session-32_2024-12-13.md"]
description: "Automated backup that runs with minimal user action after initial configuration."
---

# Plug‑and‑Forget Backup

**Definition**: A backup strategy where, once the initial folder structure and tools are set up, backup operations occur automatically without further user interaction. The goal is to make data protection "set it and forget it," reducing the chance of missed backups.

---

## Core Elements (as applied in [[summaries/session-32_2024-12-13]])
1. **Dedicated Incoming Folder** – All new media is dumped into a single, always‑present folder (e.g., *Photos Incoming*). This provides a predictable source for the backup process. See [[concepts/incoming-folder]].
2. **Automatic Cloud Sync** – A cloud service continuously mirrors the incoming folder, giving immediate off‑site protection. See [[concepts/cloud-backup]].
3. **Local Dual Copy** – The primary copy lives on the laptop, while an external drive holds a mirrored copy. The external drive is only needed occasionally; when connected, the backup runs automatically. See [[concepts/local-backup]] and [[concepts/external-drive-mirroring]].
4. **Plug‑and‑Forget Mechanism** – On Windows, the built‑in **File History** tool watches the archive folder and syncs any changes to the external drive whenever it appears. This requires no manual launch. See [[entities/file-history]] and [[concepts/plug-and-forget-backup]].
5. **Minimal Ongoing Steps** – After the initial dump, the user only needs to:
   - Perform a quick cleanup (delete junk/duplicates). See [[concepts/duplicate-removal]].
   - Create a trip‑specific folder using a consistent naming pattern (e.g., `2025‑02 Japan`). See [[concepts/trip-folder-naming]].
   - Plug in the external drive occasionally; the rest is automatic.

---

## Benefits
- **Reliability** – Backups happen every time the drive is connected, eliminating forgotten runs.
- **Low Cognitive Load** – No need to remember schedules or launch sync tasks.
- **Redundancy** – Combines cloud backup with a local external copy for layered protection.
- **Scalability** – As the archive grows, the same mechanism continues to work without extra configuration.

---

## Related Concepts
- [[concepts/backup-strategy]] – The broader plan that includes plug‑and‑forget as a component.
- [[concepts/cloud-backup]] – Provides the off‑site layer.
- [[concepts/external-drive-mirroring]] – Handles the on‑premise second copy.
- [[concepts/duplicate-removal]] – Part of the quick‑pass cleanup before archiving.
- [[concepts/trip-folder-naming]] – Ensures organized retrieval.

---

## Tools Mentioned
- **File History** (Windows) – Recommended for its seamless integration. See [[entities/file-history]].
- **FreeFileSync** – Offers more control but requires manual or scheduled activation. See [[entities/freefilesync]].

---

*Implemented based on the workflow described in [[summaries/session-32_2024-12-13]].*