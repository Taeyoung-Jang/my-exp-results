---
type: "Concept"
sources: ["summaries/session-37_2024-12-01.md"]
description: "Step-by-step guide for securely backing up data before a fresh OS install."
---

# Comprehensive Backup Checklist

**Definition**: A systematic, cross‑platform procedure for protecting personal files, application data, authentication material, and licensing information prior to a system reset or migration.

---

## Why a Checklist?
When the signs described in [[concepts/fresh-start-decision]] indicate a fresh start, having a reliable backup plan prevents data loss and reduces downtime. It also supports safe data migration as outlined in [[concepts/data-migration-safety]].

---

## Core Components
The checklist is organized into logical groups that apply to both **[[entities/windows]]** and **[[entities/macos]]** environments.

### 1. Personal Files
- Documents, photos, videos, creative projects, Desktop, Downloads.
- Store on an external drive **or** a cloud service (e.g., **[[entities/onedrive]]**, **[[entities/icloud]]**, **[[entities/google-drive]]**, **[[entities/dropbox]]**).
- macOS users may also create a full‑system Time Machine snapshot.

### 2. Browser Data
- Verify bookmarks, saved passwords, and extensions are synced to the browser account.
- If no sync, export bookmarks and passwords manually.

### 3. Application Settings & Hidden Data
- Export profiles for password managers, IDEs, creative tools, and games.
- Copy custom configuration folders:
  - Windows: `AppData\Roaming` and `AppData\Local`
  - macOS: `~/Library/Application Support`

### 4. Authentication & Security Materials
- Download or print 2FA recovery codes.
- Export SSH keys from `~/.ssh` (both OSes).
- Save VPN configuration files that are not cloud‑linked.

### 5. License & Product Keys
- Gather all software product keys and offline activation files.
- This aligns with [[concepts/license-tracking]] for future reference.

### 6. Local Email Archives
- **[[entities/outlook]]**: PST/OST files (usually in `Documents\Outlook Files`).
- **[[entities/apple-mail]]**: Mailboxes under `~/Library/Mail`.
- **[[entities/thunderbird]]**: Profiles in `~/Library/Thunderbird` (macOS) or `AppData\Roaming\Thunderbird` (Windows).

### 7. Cloud‑Sync Verification
- Open each provider’s web UI (OneDrive, iCloud, Google Drive, Dropbox) and confirm all files show as fully uploaded.
- Look for any “not synced” or paused items.

### 8. Application Inventory
- Create a concise list of essential apps to reinstall later.

### 9. OS Reinstall Preparation
- Ensure Microsoft account (Windows) or Apple ID (macOS) credentials are known.
- Optionally create bootable installation media.

### 10. Deactivate Machine‑Tied Software
- Deactivate licenses for pro apps (e.g., Adobe products) before wiping.

### 11. Final Sweep
- Scan secondary drives, VM images, Docker volumes, custom fonts, OBS profiles, and any other non‑standard storage locations.

---

## Using the Checklist
1. Follow the steps in order, checking each item off.
2. After completion, perform a quick verification by comparing the backed‑up items against the original locations on the old drive.
3. When restoring, import only the needed files (e.g., specific PST, SSH keys) to avoid re‑introducing legacy clutter—see [[concepts/data-migration-safety]].

---

## Reference
The checklist originates from the discussion in [[summaries/session-37_2024-12-01]], which details the practical experience of a full system wipe and rebuild.
