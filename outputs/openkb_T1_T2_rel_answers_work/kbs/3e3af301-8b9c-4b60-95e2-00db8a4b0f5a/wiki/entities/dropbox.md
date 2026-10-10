---
sources: ["summaries/session-37_2024-12-01.md"]
type: "Product"
description: "Dropbox is a cloud‑storage and file‑sync product mentioned in the backup checklist."
---

# Dropbox

Dropbox is a cloud‑storage and file‑synchronisation **product** that lets users keep files backed up online and access them from multiple devices.

## Key facts from [[summaries/session-37_2024-12-01]]
- Listed in the **backup checklist** (step 7) as one of the cloud‑sync services to verify that all files have been fully uploaded before a fresh‑start reset.
- Recommended to inspect the Dropbox **web interface** to confirm sync completeness, avoiding the risk of re‑importing local cache files that may contain outdated or unwanted data.
- Serves as a reference point when comparing other services such as [[entities/onedrive]], [[entities/google-drive]], and [[entities/icloud]] during the post‑rebuild sanity check.

## Relevance to concepts
- Part of the overall [[concepts/backup-checklist]] for ensuring data is safely stored before a system wipe.
- Informs [[concepts/data-migration-safety]] by highlighting the need to verify cloud sync status before importing any local‑only items.
- Can influence the [[concepts/fresh-start-decision]] when users evaluate whether their existing cloud backups (including Dropbox) are sufficient to avoid data loss.

## Practical tips (derived from the session)
1. **Check sync status**: Log into the Dropbox website and ensure no files show a “sync pending” or “offline‑only” badge.
2. **Avoid junk import**: Do not copy the local Dropbox folder back onto a freshly installed system unless you have explicitly confirmed that the cloud version is clean.
3. **Cross‑service comparison**: When auditing cloud sync completeness, repeat the same verification steps for OneDrive, Google Drive, and iCloud to maintain consistency.

---
*Entity page generated based on information from the session‑37 discussion.*