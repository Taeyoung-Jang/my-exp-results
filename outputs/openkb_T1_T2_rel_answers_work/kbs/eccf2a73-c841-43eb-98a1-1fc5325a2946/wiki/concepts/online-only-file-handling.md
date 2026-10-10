---
type: "Concept"
sources: ["summaries/session-12_2024-06-15.md"]
description: "Strategies for backing up cloud files that are stored as online‑only placeholders."
---

# Handling Online‑Only Files

**Definition:** Techniques for ensuring that files kept as "online‑only" in cloud storage are reliably backed up to a local external drive.

---

## Why online‑only matters
- Many cloud services (e.g., iCloud Drive, Google Drive) allow folders to be **online‑only** to save local disk space.
- Placeholder files exist on the Mac, but the actual data resides only on the service’s servers.
- Backup utilities can only copy files that physically exist on the machine; placeholders provide no data to copy.

---

## Core workflow (from [[summaries/session-12_2024-06-15]])
1. **Identify critical data** – Ask, “What would I miss if the cloud vanished?”
2. **Mark essential folders** as **"always keep on this device"** within the cloud app. This forces a full download of those folders so they become locally available.
3. **Run a one‑way backup** (see [[concepts/one-way-backup]]) using a tool such as [[entities/carbon-copy-cloner]] or [[entities/chronosync]] while the files are present locally.
4. **Optional manual download** – For a full‑copy of everything, temporarily download a large folder, let the backup tool copy it to the external drive, then clear the local copy to reclaim space.

---

## Key settings to avoid data loss
- **Do not enable “delete items not found at source.”** This ensures that if a file is removed from the cloud, the backup drive keeps the last known copy.
- **Enable versioning or archive mode** in the backup tool so that overwritten files are retained (e.g., SafetyNet in Carbon Copy Cloner).

---

## Trade‑offs
| Option | Pros | Cons |
|--------|------|------|
| Keep only key folders local | Saves Mac storage, automatic backup of important items | Requires manual selection of what’s important |
| Download everything before backup | Guarantees a complete offline copy | Requires sufficient local disk space, may be cumbersome |

---

## Related concepts
- [[concepts/cloud-storage-vs-external-drive]] – explains why a hybrid strategy often uses the cloud as the source of truth.
- [[concepts/one-way-backup]] – details the safest backup direction to prevent accidental deletions.

---

## Practical tip for macOS users
On **macOS**, use the Finder view for the cloud service and right‑click a folder → *"Always keep on this device"*. After the download finishes, run your chosen backup task and then you may switch the folder back to *online‑only* if you need to reclaim space.
