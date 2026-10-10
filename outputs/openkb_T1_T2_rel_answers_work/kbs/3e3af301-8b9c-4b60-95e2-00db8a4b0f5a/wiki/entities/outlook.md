---
sources: ["summaries/session-37_2024-12-01.md"]
type: "Product"
description: "Microsoft Outlook is a Windows email client for managing PST archives and calendars."
---

# Microsoft Outlook

## Overview
Microsoft Outlook is a desktop email, calendar, and contacts application primarily for the Windows operating system. It stores local mail data in PST (Personal Storage Table) files and integrates with Microsoft 365 services.

## Role in [[summaries/session-37_2024-12-01]]
In the session‑37 guide, Outlook is highlighted as one of the key local‑only data sources that must be backed up before a fresh‑start reset. The document advises locating PST files either in **Documents\Outlook Files** or in **%AppData%\Local\Microsoft\Outlook** and copying them to a safe backup location.

## Backup considerations
- Include Outlook PST/OST files in the [[concepts/backup-checklist]] to ensure no email history is lost.
- Verify that any exported archives are stored on external media or cloud storage before reinstalling the OS.

## Data migration safety
When moving to a new installation, follow the [[concepts/data-migration-safety]] steps: import the saved PST files via Outlook’s *Import/Export* wizard rather than simply copying files into the application data folders.

## License and activation
Outlook is part of the Microsoft 365 suite; handling its license falls under [[concepts/license-tracking]]. Ensure the Microsoft account credentials are known and that any offline activation files (if used) are saved.

## Related entities
- [[entities/windows]] – the operating system Outlook runs on.

---
*Entity page generated from the discussion in [[summaries/session-37_2024-12-01]].*