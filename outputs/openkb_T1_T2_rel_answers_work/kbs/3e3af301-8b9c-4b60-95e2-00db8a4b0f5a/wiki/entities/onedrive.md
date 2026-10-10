---
sources: ["summaries/session-37_2024-12-01.md"]
type: "Product"
description: "Microsoft's cloud storage and syncing service for Windows and macOS."
---

# Microsoft OneDrive

Microsoft OneDrive is a cloud‑based file storage and synchronization service that integrates tightly with **Windows** and is also available on **macOS**. It is commonly used in personal and professional backup workflows.

## Role in the Fresh‑Start Process
- Listed in the **[[concepts/backup-checklist]]** as a key cloud‑sync provider that must be verified as fully uploaded before a system reset.
- The document advises checking the OneDrive web interface for any files marked "not synced" or "sync paused" to avoid losing locally‑only data.
- OneDrive is mentioned alongside other services such as **[[entities/icloud]]**, **[[entities/google-drive]]**, and **[[entities/dropbox]]** when confirming cloud‑sync completeness.

## Safety Considerations for Data Migration
- Treat OneDrive as part of the **[[concepts/data-migration-safety]]** strategy: inspect the old drive for leftover OneDrive caches but import only the necessary files via the web UI or a fresh client install.
- When rebuilding a machine, avoid pulling in old OneDrive cache folders that may contain outdated or junk files; instead, let the new client resync from the cloud after confirming the cloud version is complete.

## Connection to Session‑37 Guidance
- The checklist in **[[summaries/session-37_2024-12-01]]** emphasizes confirming that OneDrive (and other sync services) show a fully synchronized state before proceeding with a reset.
- It also suggests using OneDrive alongside other backup steps such as exporting local email archives, SSH keys, and 2FA recovery codes.

## Key Facts
- Integrated with the Windows file explorer for seamless drag‑and‑drop sync.
- Provides personal (free) and business (Office 365) plans.
- Supports version history, which can be useful when recovering mistakenly overwritten files after a fresh start.

---
*Entity type*: product