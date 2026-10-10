---
sources: ["summaries/session-12_2024-06-15.md"]
type: "Product"
description: "Carbon Copy Cloner is a macOS backup utility for one‑way, versioned copying."
---

## Carbon Copy Cloner (product)

**Carbon Copy Cloner** (often abbreviated as CCC) is a commercial backup application for **macOS** that creates one‑way copies of selected source folders to a destination drive, while preserving previous versions of files in an archive (SafetyNet).

### Key points from [[summaries/session-12_2024-06-15]]
- Recommended as a primary tool for a **one‑way backup** workflow when the cloud storage is the source of truth. 
- Configured in *copy* mode rather than *mirror* to avoid deletions on the destination.
- The **SafetyNet** feature should be enabled so that older or replaced files are retained, providing versioned backups.
- Works well with folders that are fully synced locally on a Mac, making it suitable for users who keep critical cloud folders set to “always keep on this device.”

### How it fits the backup strategy
- Aligns with the concept of [[concepts/one-way-backup]] by ensuring data flows only from the cloud‑synced folder to the external drive, never the reverse.
- Complements the decision framework of [[concepts/cloud-storage-vs-external-drive]] by offering granular control over what gets backed up and how versions are retained.
- When dealing with **online‑only** cloud files, CCC can only back up what is present locally; therefore users should mark essential folders for local availability as described in [[concepts/online-only-file-handling]].

### Comparison with alternatives
- **ChronoSync** (see [[entities/chronosync]]) offers a similar left‑to‑right backup mode, but CCC’s SafetyNet is praised for its ease of use.
- **Time Machine** (see [[entities/time-machine]]) provides built‑in versioned backups but requires all cloud files to be locally present, which may not be the case for online‑only items.

### Typical workflow for macOS users
1. Ensure the cloud storage app syncs the chosen folders locally on **macOS** (see [[entities/macos]]).  
2. Create a CCC task: *Source* = cloud‑synced folder, *Destination* = external drive.  
3. Set the task type to **Copy** (not Mirror).  
4. Enable **SafetyNet** to archive older versions.  
5. Schedule the task to run periodically (e.g., weekly) when the drive is connected.

### Why use Carbon Copy Cloner?
- Provides reliable, versioned backups without risking accidental sync‑back to the cloud.
- Offers fine‑grained control over which folders are backed up and how many historical versions to retain.
- Simple UI that integrates smoothly with macOS and external drive workflows.

---
*This entity page consolidates the role of Carbon Copy Cloner as described in the session‑12 discussion, linking it to relevant concepts and comparative tools.*