---
sources: ["summaries/session-37_2024-12-01.md"]
type: "Product"
description: "Apple's desktop operating system for Mac computers."
---

# macOS

**Type:** product

macOS is Apple's proprietary operating system for Mac hardware. In the context of [[summaries/session-37_2024-12-01]], macOS is discussed as one of the two target platforms (the other being Windows) for a systematic fresh‑start workflow.

## Key Points from the Session

- **When to consider a fresh start** – The session links the decision to the [[concepts/fresh-start-decision]] model, noting that persistent performance issues, repeated crashes, or an unmanageable tangle of legacy software are strong signals.
- **Backup checklist** – A detailed macOS‑specific backup checklist is provided, aligning with [[concepts/backup-checklist]]. Steps include:
  1. Back up personal files (Documents, Desktop, Downloads) to an external drive or cloud (Time Machine is highlighted as a macOS‑specific full‑system snapshot tool).
  2. Ensure browser data is synced (Safari, Chrome, Firefox) and export bookmarks/passwords if sync is disabled.
  3. Export hidden app data from `~/Library/Application Support/` for tools that don’t auto‑sync.
  4. Save authentication material: 2FA recovery codes, SSH keys from `~/.ssh`, VPN configs.
  5. Gather license keys and offline activation files (see [[concepts/license-tracking]]).
  6. Preserve local email archives from [[entities/apple-mail]] (found under `~/Library/Mail`).
  7. Verify cloud‑sync completeness for services such as [[entities/icloud]], [[entities/google-drive]], [[entities/dropbox]], and [[entities/onedrive]].
  8. List essential apps to reinstall later.
  9. Prepare OS reinstall media (Apple ID credentials, optional bootable installer).
  10. Deactivate machine‑tied software before wiping.
  11. Perform a final sweep for custom folders, VM images, Docker volumes, fonts, and other non‑standard data locations.
- **Post‑rebuild sanity check** – The session outlines a safe verification process that falls under [[concepts/data-migration-safety]]. It recommends mounting the old drive read‑only, inspecting typical macOS locations:
  - `~/.ssh` for SSH keys
  - `~/Library/Mail` for Apple Mail archives
  - `~/Library/Thunderbird` for Thunderbird profiles
  - `~/Library/Application Support/<vendor>` for license files and activation data
  - User folders (Documents, Desktop, Downloads) for manually stored 2FA recovery codes.
- **Safe transfer method** – Copy only the identified needed files to a temporary folder on the new macOS installation and import them using the appropriate application’s import function (e.g., import Mail mailboxes via Apple Mail, add SSH keys with correct permissions).

## Related Concepts and Entities

- [[concepts/backup-checklist]] – The overarching framework for preparing a system reset.
- [[concepts/fresh-start-decision]] – Criteria for deciding when a clean install is warranted.
- [[concepts/data-migration-safety]] – Guidelines for verifying completeness and avoiding junk re‑introduction.
- [[concepts/license-tracking]] – Managing software keys and activation files.
- [[entities/apple-mail]] – Local email client discussed for archive extraction.
- [[entities/icloud]] – Cloud service used for file and photo sync.
- [[entities/google-drive]], [[entities/dropbox]], [[entities/onedrive]] – Alternative cloud sync providers mentioned.
- [[entities/windows]] – The counterpart OS used for comparison in the checklist.

---
*This entity page is derived from the discussion in [[summaries/session-37_2024-12-01]].*