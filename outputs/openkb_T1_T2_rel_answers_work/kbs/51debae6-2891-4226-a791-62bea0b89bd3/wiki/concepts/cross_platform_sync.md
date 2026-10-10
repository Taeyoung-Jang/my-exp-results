---
type: "Concept"
sources: ["summaries/session-38_2025-10-15.md"]
description: "Method for keeping data synchronized across devices using a single ecosystem."
---

# Cross‑Platform Sync

**Definition**: Cross‑platform sync is the practice of using a single [[concepts/source_of_truth]] or [[concepts/ecosystem]] to store calendars, contacts, notes, and photos so that they automatically stay consistent across multiple devices such as an [[entities/iphone]], a laptop (e.g., [[entities/windows]]), and a tablet.

## Core Principles
1. **Pick one ecosystem** – either Apple’s iCloud or Google’s services become the master repository for personal data. This reduces friction and eliminates the need for manual reconciliation.
2. **Enable only necessary sync categories** – on each device, activate only the data types (Contacts, Calendars, Notes, Photos) that belong to the chosen ecosystem.
3. **Disable competing services** – turn off iCloud sync for Contacts and Calendars when using Google, and vice‑versa, to prevent duplicate records. This aligns with the [[concepts/duplicate_avoidance]] approach.
4. **Set default account** – on iOS, set the default contacts account to the chosen ecosystem (e.g., Google) so new entries are created in the correct database.

## Practical Steps from Session 38
- **iPhone + Windows using Google**
  - Add the Google account in iOS Settings → Accounts.
  - Toggle **Contacts** and **Calendars** on; keep **Photos** handled by Google Photos.
  - Set Google as the default contacts store.
  - On Windows, use Google’s web or desktop apps; no extra configuration needed.

- **Photo handling**
  - Google Photos works on iPhone but resides separately from the native Photos app, meaning the device maintains a local camera roll in addition to the cloud backup.
  - iCloud Photos integrates directly with the iOS Photos app, offering seamless handling of Live Photos and original‑resolution files.

- **Migrating existing iCloud data**
  1. Export contacts from iCloud.com as a vCard and import into Google Contacts.
  2. Export iCloud calendars and import them into Google Calendar.
  3. Verify the data on the iPhone, then disable iCloud sync for Contacts and Calendars.

- **When an IT‑provided cross‑platform system is already in place**
  - Align any remaining iCloud items with the IT‑standard system instead of a separate Google migration, then disable iCloud syncing to avoid duplicate sources of truth.

## Related Concepts
- [[concepts/duplicate_avoidance]] – strategies to prevent duplicate records when multiple sync services are active.
- [[concepts/mixing_and_matching]] – combining features from different ecosystems while maintaining a single source of truth.
- [[concepts/smartwatch_integration]] – extending cross‑platform sync to wearables (e.g., Fitbit, Garmin) that rely on the same ecosystem.

## Source Document
- [[summaries/session-38_2025-10-15]]