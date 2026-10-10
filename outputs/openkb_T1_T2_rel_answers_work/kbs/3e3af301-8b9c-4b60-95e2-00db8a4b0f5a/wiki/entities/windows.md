---
sources: ["summaries/session-37_2024-12-01.md"]
type: "Product"
description: "Microsoft's flagship operating system for PCs."
---

# Windows

Windows is Microsoft’s primary desktop operating system, widely used on personal computers. In the context of [[summaries/session-37_2024-12-01]], Windows is referenced as one of the two platforms (the other being macOS) for which a comprehensive [[concepts/fresh-start-decision]] and [[concepts/backup-checklist]] are provided.

## Key Points from Session 37

- **When to consider a fresh start**: Persistent performance issues, recurring crashes, or an unclear root cause are highlighted as signals that a reset or reinstall may be more efficient than continued troubleshooting.
- **Backup checklist**: The document outlines a step‑by‑step process covering personal files, browser data, app settings, authentication materials (including 2FA recovery codes and SSH keys), license information, local email archives (e.g., Outlook PST files), and cloud‑sync verification. This aligns with the [[concepts/backup-checklist]] concept.
- **Local‑only data locations**: Specific Windows paths are mentioned for locating items that do not automatically sync:
  - `C:\Users\<user>\.ssh` for SSH keys
  - `Documents\Outlook Files` and `AppData\Local\Microsoft\Outlook` for Outlook PST/OST files
  - `AppData\Roaming\Thunderbird\Profiles` for Thunderbird data
  - `AppData\Roaming\<vendor>` or `ProgramData\<vendor>` for license or activation files
- **Cloud‑sync verification**: Emphasizes checking OneDrive, Dropbox, Google Drive, and other services via their web interfaces to ensure completeness without re‑importing stale data, tying into the [[concepts/data-migration-safety]] concept.
- **Safe migration**: Recommends copying only the needed files (e.g., a single PST or SSH key) to a neutral location on the new system and using each application’s import routine, supporting the [[concepts/data-migration-safety]] practice.

## Related Entities and Concepts

- Compared with [[entities/macos]] for cross‑platform considerations.
- Cloud storage services mentioned include [[entities/onedrive]], [[entities/dropbox]], and [[entities/google-drive]].
- Email client references include [[entities/outlook]] and [[entities/thunderbird]].
- License tracking is linked to the [[concepts/license-tracking]] concept.

## See Also

- [[summaries/session-37_2024-12-01]] – Full discussion of Windows backup and migration steps.
- [[concepts/fresh-start-decision]] – Decision criteria for reinstalling an OS.
- [[concepts/backup-checklist]] – Detailed checklist used for Windows and macOS.
- [[concepts/data-migration-safety]] – Guidelines for safely moving data.
- [[concepts/license-tracking]] – Managing software license files on Windows.