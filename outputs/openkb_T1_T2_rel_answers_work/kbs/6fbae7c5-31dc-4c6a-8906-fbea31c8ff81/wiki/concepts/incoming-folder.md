---
type: "Concept"
sources: ["summaries/session-32_2024-12-13.md"]
description: "A dedicated folder where new media is initially dumped for easy processing and backup."
---

## Incoming Folder

**Definition**: An *Incoming Folder* is a permanent, top‑level directory on a computer where all newly transferred photos and videos are placed immediately after a trip, before any sorting or backup steps.

### Why it matters
- Provides a single, predictable location for all fresh media, eliminating the need to decide where each file goes.
- Enables automated tools (cloud sync, File History, etc.) to monitor one path for continuous backup.
- Serves as the starting point for a quick cleanup routine and subsequent organization into named trip folders.

### How to set up (based on [[summaries/session-32_2024-12-13]])
1. **Create the folder** – On a Windows laptop, make a folder such as `C:\Photos Incoming`.
2. **Use it consistently** – Every time you plug in a phone, camera, or SD card, **dump all files directly into this folder** without pre‑sorting.
3. **Leave it for automation** – Let cloud backup services (OneDrive, Google Photos, etc.) sync this folder automatically.
4. **Run a fast clean‑up** – After the cloud copy finishes, quickly delete obvious junk, duplicates, or blurred shots.
5. **Move to a trip folder** – Drag the cleaned set into a sub‑folder named with date and location (e.g., `2025-02 Japan`).

### Related concepts
- [[concepts/cloud-backup]] – The automatic cloud sync that watches the Incoming Folder.
- [[concepts/duplicate-removal]] – The quick pass to delete unwanted files after the initial dump.
- [[concepts/trip-folder-naming]] – The naming convention for the final, organized trip folders.
- [[concepts/external-drive-mirroring]] – The process that later copies the organized archive to an external drive.
- [[concepts/plug-and-forget-backup]] – The overall low‑maintenance backup approach enabled by a stable Incoming Folder.

### Benefits
- **Simplicity** – No need to think about folder structure during the initial transfer.
- **Reliability** – Guarantees that every file is captured by backup services.
- **Scalability** – Works for any volume of media; later steps can be performed at leisure.

---
*This concept is illustrated in the workflow described in [[summaries/session-32_2024-12-13]].*