---
sources: ["summaries/session-37_2024-12-01.md"]
type: "Product"
description: "Cross‑platform email client that stores local mail archives in user profiles."
---

## Mozilla Thunderbird

Mozilla Thunderbird is a free, open‑source email client available for Windows and macOS. It stores all user data—including account settings, local mail archives, and extensions—in a **profile folder** that lives in the user’s application data directory.

### Key facts from [[summaries/session-37_2024-12-01]]
- **Profile locations**:
  - **Windows**: `C:\Users\<user>\AppData\Roaming\Thunderbird\Profiles\<profile>`
  - **macOS**: `/Users/<user>/Library/Thunderbird/Profiles/<profile>`
- The document emphasizes backing up this folder as part of a comprehensive [[concepts/backup-checklist]] when planning a [[concepts/fresh-start-decision]].
- Local email archives (PST/mbox files) stored in the Thunderbird profile are considered *local‑only data* that must be saved before a system reset.
- When migrating to a fresh system, the checklist advises copying only the necessary profile sub‑folders (e.g., `Mail`, `ImapMail`, `prefs.js`) to avoid bringing in unwanted legacy settings, aligning with [[concepts/data-migration-safety]].

### Related entities and platforms
- Works on [[entities/windows]] and [[entities/macos]].
- Often used alongside other email clients such as [[entities/outlook]] and [[entities/apple-mail]].

### Practical guidance
1. **Backup**: Include the entire Thunderbird profile folder in your backup routine.
2. **Verify**: After a fresh install, import the saved profile via Thunderbird’s profile manager rather than copying the whole directory.
3. **Safety**: Transfer only the essential sub‑folders to keep the new system clean, following the principles of [[concepts/data-migration-safety]].

For a full checklist and more details on preparing for a clean system reinstall, see the session summary.