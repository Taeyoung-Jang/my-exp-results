---
type: "Concept"
sources: ["summaries/session-32_2024-12-13.md", "summaries/session-07_2024-06-15.md"]
description: "Cloud backup stores phone data online for automatic, cross‑device recovery."
---

# Cloud Backup

**Definition**: Cloud backup is a service that continuously copies selected phone data (photos, notes, messages, etc.) to remote servers, enabling recovery without needing a physical device.

## Overview
- Runs in the background and updates automatically.
- Provides instant access to data on a new device by signing into the same account.
- Central to a robust [[concepts/backup-strategy]] when combined with [[concepts/local-backup]].

## Benefits
- **Convenience** – No manual steps after initial setup.
- **Recovery Speed** – Restores data directly from the cloud to a replacement phone.
- **Device Agnostic** – Works across iPhone and Android platforms.

## Trade‑offs
- **Storage Limits** – Free tiers have caps; larger libraries may need a paid plan.
- **Subscription Cost** – Ongoing fee for extra space (e.g., [[entities/google-one]] or Apple iCloud plans).
- **Trust** – Relies on third‑party providers to safeguard privacy and uptime.

## Platform‑Specific Details (from [[summaries/session-07_2024-06-15]])
### iPhone (iCloud)
- Enable via **Settings → \[your name\] → iCloud → iCloud Backup**.
- Verify **Photos** (iCloud Photos), **Notes**, and **Messages in iCloud** are toggled on.
- Check the **Last successful backup** timestamp.
- Service is provided by [[entities/icloud]] (Apple).

### Android (Google)
- Enable via **Settings → System → Backup**; look for **Backup by Google One** status.
- Turn on **Google Photos** backup (provided by [[entities/google-photos]]) and ensure recent activity.
- For notes, use **Google Keep** ([[entities/google-keep]]) and confirm sync on keep.google.com.
- Messages rely on RCS and system‑level backup; ensure RCS is active.
- Service is tied to a [[entities/google]] account.

## Monitoring & Quick Checks
- Regularly inspect the backup status line or **Last backup** date.
- Compare item counts (photos, notes) on the device vs. the cloud dashboard.
- Spot‑check recent uploads via the web interface (iCloud.com, photos.google.com, keep.google.com).

## Relation to Other Concepts
- Works hand‑in‑hand with [[concepts/local-backup]] to create a layered protection model.
- Forms the core of a comprehensive [[concepts/backup-strategy]] for mobile data.


See also: [[summaries/session-32_2024-12-13]]