---
sources: ["summaries/session-12_2024-06-15.md"]
type: "Product"
description: "Apple's built‑in macOS backup utility that creates incremental snapshots."
---

# Time Machine (product)

**Type:** product

**Description:** Apple’s built‑in macOS backup utility that creates incremental snapshots of your files and allows versioned restores.

## Core features
- Automatic hourly, daily, and weekly backups to a designated external drive.
- Incremental, versioned backups that let you restore previous file versions.
- Seamless integration with macOS Finder and System Preferences.

## Relevance to session-12_2024-06-15
- Recommended as a *simple* backup solution for users who keep their cloud‑storage files fully synced locally on macOS.
- Noted as having a limitation: it can only back up files that are present on the local disk, so “online‑only” placeholders from cloud services are not captured.
- Compared with third‑party one‑way backup tools such as [[entities/carbon-copy-cloner]] and [[entities/chronosync]], which can handle cloud folders that are not fully downloaded.
- Mentioned alongside the concept of [[concepts/one-way-backup]] and the need to avoid reverse syncing when creating a backup.

## Related concepts and entities
- [[concepts/cloud-storage-vs-external-drive]] – the broader decision framework in which Time Machine is a possible option.
- [[concepts/one-way-backup]] – the backup style recommended for the external drive.
- [[concepts/online-only-file-handling]] – a limitation of Time Machine when dealing with cloud‑only files.
- [[entities/carbon-copy-cloner]] – an alternative tool for one‑way, versioned backups.
- [[entities/chronosync]] – another alternative backup utility.
- [[entities/macos]] – the operating system on which Time Machine runs.

## Source summary
- For a full discussion of how Time Machine fits into the suggested workflow, see [[summaries/session-12_2024-06-15]].