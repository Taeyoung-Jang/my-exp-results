---
sources: ["summaries/session-37_2024-12-01.md"]
type: "Product"
description: "Apple Mail is macOS's built‑in email client."
---

# Apple Mail (product)

Apple Mail is the default email client bundled with macOS, providing a native interface for managing local and iCloud‑synced mailboxes.

## Key facts from [[summaries/session-37_2024-12-01]]
- **Local archives location**: Mail data is stored on disk at `~/Library/Mail`.  This folder holds the on‑disk representation of mailboxes, attachments, and account settings that are not automatically synced via iCloud.
- **Backup considerations**: When planning a fresh‑start or system reinstall, the document advises explicitly checking the `~/Library/Mail` directory for local‑only archives and copying any needed PST‑like files before wiping the drive.
- **Typical usage pattern**: Users often rely on iCloud sync for mail, but any manually‑added accounts (e.g., corporate IMAP/POP) may retain messages only in the local mailbox folder, making it essential to back up this location.

## Related concepts
- [[concepts/backup-checklist]] – includes the step to back up local email archives such as Apple Mail's `~/Library/Mail`.
- [[concepts/fresh-start-decision]] – decision points that may trigger a reinstall where Apple Mail data must be preserved.
- [[concepts/data-migration-safety]] – safe methods for transferring specific Apple Mail files without bringing in unwanted settings.

## Related entities
- [[entities/macos]] – the operating system that ships with Apple Mail.
- [[entities/icloud]] – the cloud service often used to sync Apple Mail data across devices.
