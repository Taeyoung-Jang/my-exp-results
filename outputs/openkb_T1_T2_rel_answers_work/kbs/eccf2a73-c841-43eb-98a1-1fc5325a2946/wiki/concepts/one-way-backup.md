---
type: "Concept"
sources: ["summaries/session-12_2024-06-15.md"]
description: "Procedure to copy cloud data to an external drive without reverse syncing."
---

# One‑Way Backup Workflow

**Definition**: A one‑way backup workflow copies data from a source (typically cloud storage) to a destination (usually an external drive) while guaranteeing that no changes flow back to the source, preserving the source as the single point of truth.

---

## Why Use a One‑Way Workflow?
- Prevents accidental deletion or modification of cloud files by the backup destination.
- Provides a reliable safety net that can be versioned without affecting daily operations.
- Complements a hybrid storage strategy where the cloud serves as the authoritative data store.

## Core Components
| Component | Role |
|-----------|------|
| **Source** | Cloud storage folders that are kept in sync locally on [[entities/macos]]. |
| **Destination** | External hard drive that stores the backup copy. |
| **Tool** | Software that performs a unidirectional copy. Recommended options are [[entities/carbon-copy-cloner]] and [[entities/chronosync]]; [[entities/time-machine]] can be used only if all cloud files are fully downloaded. |

## Recommended Tools & Settings
- **Carbon Copy Cloner (CCC)**
  - Create a **Copy** task (not a Mirror).
  - Enable **SafetyNet** to archive older versions of overwritten files.
  - Ensure the option *“Delete items not found at the source”* is **disabled**.
- **ChronoSync**
  - Choose **Left‑to‑Right** backup mode.
  - Turn off *Deletion* for items missing on the left side.
  - Activate the **Archive** feature to keep previous versions.
- **Time Machine**
  - Viable only when the cloud folders are stored locally (no placeholders).
  - Works out‑of‑the‑box with versioning but cannot back up online‑only files.

## Step‑by‑Step Workflow
1. **Define the source of truth** – Decide that the cloud storage hierarchy is the master structure (see [[concepts/cloud-storage-vs-external-drive]]). 
2. **Local sync** – Ensure the cloud client on [[entities/macos]] has the needed folders set to *always keep on this device* (addresses [[concepts/online-only-file-handling]]). 
3. **Configure the backup task** – In CCC or ChronoSync, point the source to the local cloud folder and the destination to the external drive. Apply the safety/archive settings described above. 
4. **Schedule regular runs** – Run the task weekly or after major changes. Connect the drive, let the tool finish, then disconnect. 
5. **Verify** – Periodically inspect the archive folder to confirm older versions are retained and that no files have been removed from the drive unintentionally.

## Handling Online‑Only Files
If certain cloud items are stored as placeholders to save local disk space, they must be downloaded before the backup runs. Options:
- Mark critical folders as **always local** in the cloud client.
- Manually trigger a download of a large folder, run the backup, then optionally clear the local copy.
This trade‑off is inherent to [[concepts/online-only-file-handling]].

## Benefits of the Workflow
- **Safety**: The external drive never writes back to the cloud.
- **Versioning**: Older file versions are kept in an archive, allowing recovery from accidental edits.
- **Simplicity**: Once set up, the process requires only plugging in the drive and letting the tool run.

---

## Reference
The workflow is distilled from the discussion in [[summaries/session-12_2024-06-15]], which explored practical backup setups for macOS users handling mixed cloud and local storage.
