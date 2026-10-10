---
type: "Concept"
sources: ["summaries/session-38_2025-10-15.md"]
description: "Techniques to prevent duplicate contacts, calendars, and data across synced services."
---

# Duplicate Avoidance

**Definition**: Methods and best‑practice configurations that ensure a single source of truth for contacts, calendars, notes, and photos, eliminating redundant or conflicting entries when syncing across multiple devices and platforms.

---

## Why It Matters

When users operate across an **iPhone**, a **Windows** laptop, and possibly other devices, enabling multiple cloud services (e.g., iCloud and Google) can cause duplicate records. Duplicate data leads to confusion, missed appointments, and wasted storage.

The concept is closely tied to [[concepts/source_of_truth]], [[concepts/ecosystem]], and [[concepts/cross_platform_sync]].

---

## Core Strategies (from [[summaries/session-38_2025-10-15]])

1. **Select a single ecosystem as the master** – either iCloud or Google. This becomes the *source of truth* for contacts and calendars.
2. **Configure device accounts deliberately**:
   - On the **iPhone**, add the chosen Google account in Settings → Accounts.
   - Enable **only** *Contacts* and *Calendars* for that account.
   - Set the default contacts account to Google (Settings → Contacts → Default Account).
   - Turn **off** iCloud contacts and calendar sync to stop parallel databases.
3. **Migrate existing data safely**:
   - Export iCloud contacts as a vCard and import them into Google Contacts.
   - Export iCloud calendars (ICS) and import them into Google Calendar.
   - Verify the imported data on all devices before disabling iCloud sync.
4. **Maintain the chosen ecosystem**:
   - For future additions, always create contacts/events in the default Google account.
   - Periodically audit for stray iCloud entries and delete them.
5. **Photo considerations** – While not a direct duplicate issue, using Google Photos on iPhone keeps a separate local camera roll; understanding this helps avoid confusion about where new photos reside.

---

## Related Concepts

- [[concepts/source_of_truth]] – establishing a single authoritative data store.
- [[concepts/ecosystem]] – choosing iCloud vs. Google as the primary platform.
- [[concepts/cross_platform_sync]] – keeping data consistent across iPhone, Windows, and other devices.
- [[concepts/mixing_and_matching]] – when and why blending services can re‑introduce duplication risks.

---

## Practical Tips

- **Use defaults**: Always set the default account for contacts and calendars to the chosen ecosystem.
- **Disable competing services**: In Settings, toggle off iCloud sync for categories you have migrated.
- **One‑time export/import**: Perform a single migration rather than incremental syncs to avoid partial duplicates.
- **Audit regularly**: A quick check of the contacts app and calendar list can reveal stray entries before they proliferate.

---

By following these steps, users can achieve reliable **duplicate avoidance** and enjoy seamless data access without manual reconciliation.