---
type: "Concept"
sources: ["summaries/session-37_2024-12-01.md"]
description: "Guidelines for securely moving personal data during system resets without exposing junk."
---

# Safe Data Migration Practices

**Definition**: A set of procedures that ensure only the intended personal files, credentials, and configuration data are transferred when reinstalling or resetting a computer, while preventing accidental migration of obsolete or unwanted artifacts.

---

## Why it matters
When a user decides on a [[concepts/fresh-start-decision]]—for example because of persistent performance issues or tangled software configurations—migrating data safely is crucial to retain productivity and security. The practice builds on the broader [[concepts/backup-checklist]] but focuses on the *transfer* phase, not just the backup phase.

---

## Core Steps (derived from [[summaries/session-37_2024-12-01]])

1. **Identify local‑only locations**
   - Windows: `C:\Users\<user>\.ssh`, Outlook files in `Documents\Outlook Files` or `AppData\Local\Microsoft\Outlook`, Thunderbird profiles in `AppData\Roaming\Thunderbird\Profiles`, vendor license folders in `AppData\Roaming` or `ProgramData`.
   - macOS: `~/ .ssh`, Mail in `~/Library/Mail`, Thunderbird in `~/Library/Thunderbird`, app‑specific support in `~/Library/Application Support` or `/Library/Application Support`.
   - Common stash spots for 2FA recovery codes: Documents, Desktop, Downloads, or custom "Security" folders.

2. **Verify cloud‑sync completeness**
   - Open each provider’s web console (e.g., [[entities/icloud]], [[entities/google-drive]], [[entities/onedrive]], [[entities/dropbox]]) and confirm that the file list shows *fully uploaded* items, no pending sync warnings, and that libraries such as iCloud Photos or Google Photos are complete.

3. **Isolate needed items**
   - For each category (SSH keys, PST/MBX archives, license files, 2FA codes) copy *only the specific file or sub‑folder* to a neutral holding folder on the new system. Do **not** copy entire parent directories.
   - Example: copy `id_rsa` and `id_rsa.pub` from the old `.ssh` folder, not the whole `.ssh` directory.

4. **Import using the target application’s proper routine**
   - Outlook: use *File → Open & Export → Import/Export* to bring in PST files.
   - Thunderbird: place the profile folder under `~/Library/Thunderbird` and start the app.
   - Apple Mail: import the `Mail` directory via the Mail app’s *Import Mailboxes*.
   - SSH: place keys in the new `~/.ssh` folder, set permissions `600` for private keys, `644` for public keys.
   - License files: copy the exact license file to the expected location (often under `AppData\Roaming\<vendor>` on Windows or `~/Library/Application Support/<vendor>` on macOS) and re‑activate if necessary.

5. **Final validation**
   - Run a quick audit of the new system: check that all expected keys, archives, and licenses are present and functional.
   - Ensure no stray old configuration files remain on the drive (e.g., leftover `AppData\Local` junk, old VM images, or lingering Docker volumes).

---

## Relationship to other concepts
- Part of a comprehensive [[concepts/backup-checklist]] before a reset.
- Directly implements the safety principles described in [[concepts/data-migration-safety]].
- Complements [[concepts/license-tracking]] by ensuring license files are deliberately moved.

---

## Relevant entities
- Operating systems: [[entities/windows]], [[entities/macos]]
- Email clients: [[entities/outlook]], [[entities/apple-mail]], [[entities/thunderbird]]
- Cloud services: [[entities/icloud]], [[entities/google-drive]], [[entities/onedrive]], [[entities/dropbox]]

---

**Note**: This concept is anchored in the real‑world workflow outlined in [[summaries/session-37_2024-12-01]], which provides the concrete checklist and verification tactics.
