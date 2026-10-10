---
type: "Concept"
sources: ["summaries/session-32_2024-12-13.md"]
description: "Automatic syncing of a photo archive to an external drive for redundant local backup."
---

# External Drive Mirroring

External Drive Mirroring is a **plug‑and‑forget** method for creating a second local copy of a photo or video archive on an external storage device. The goal is to keep the primary collection on the computer while maintaining an up‑to‑date duplicate on a removable drive, providing redundancy without manual intervention.

## How it works (based on [[summaries/session-32_2024-12-13]])
1. **Single archive folder** – All trips are stored in a consistent folder structure (e.g., a "Photos" folder with sub‑folders named by date and location). This satisfies the [[concepts/incoming-folder]] and [[concepts/trip-folder-naming]] requirements.
2. **Automatic sync** – A background backup tool watches the archive folder and mirrors any changes to the external drive whenever it is connected.
3. **Tools** – On Windows, the recommended tool is **File History** ([[entities/file-history]]), which automatically detects the external drive and updates the backup without user action. An alternative with more control is **FreeFileSync** ([[entities/freefilesync]]), but it typically needs a scheduled task or manual launch.
4. **Redundancy** – Together with a cloud service (see [[concepts/cloud-backup]]), the external drive provides a second local copy, forming a robust [[concepts/backup-strategy]] that protects against both device failure and cloud‑service outages.

## Key Benefits
- **Low maintenance** – Once configured, the process runs automatically each time the drive is plugged in, aligning with the [[concepts/plug-and-forget-backup]] principle.
- **Immediate protection** – New or edited files are captured without waiting for a manual sync, ensuring the external copy stays current.
- **Simple recovery** – If the laptop drive fails, the external mirror can be swapped in instantly, avoiding complex restoration steps.

## Typical Setup Steps
1. Create a permanent "Photos Incoming" (or similar) folder on the laptop.
2. Enable **File History** via Windows Settings:
   - Select the photo archive folder as the source.
   - Choose the external drive as the backup destination.
   - Ensure the schedule is set to run continuously or at frequent intervals.
3. (Optional) If using **FreeFileSync**, create a sync job that mirrors the archive folder to the external drive and schedule it to run on drive connection.

## Related Concepts
- [[concepts/backup-strategy]] – Overall approach combining cloud and local copies.
- [[concepts/cloud-backup]] – Complementary remote copy of the same archive.
- [[concepts/local-backup]] – The broader category of storing data on local hardware.
- [[concepts/duplicate-removal]] – Cleaning up files before they are mirrored to avoid unnecessary storage usage.
- [[concepts/incoming-folder]] – The initial staging area for new media.
- [[concepts/trip-folder-naming]] – Consistent naming that aids automated syncing.

By implementing External Drive Mirroring, users can achieve a reliable, hands‑free backup routine that keeps their travel memories safe across both cloud and physical media.