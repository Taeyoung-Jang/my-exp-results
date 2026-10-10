---
type: "Concept"
sources: ["summaries/session-38_2025-10-15.md"]
description: "Central account that holds the master copy of data for sync across devices."
---

# Source of Truth

**Definition**: A *source of truth* is the single, authoritative account or service where the master copy of a user’s data (contacts, calendars, notes, photos, etc.) resides, and from which all devices and apps synchronize.

## Why it matters
- Prevents **[[concepts/duplicate_avoidance]]** by ensuring only one system creates or modifies records.
- Enables reliable **[[concepts/cross_platform_sync]]** across phones, laptops, and tablets.
- Simplifies management: changes made on any device propagate automatically.

## Guidance from [[summaries/session-38_2025-10-15]]
- Choose either **[[entities/icloud]]** (ideal for iPhone/macOS users) or **[[entities/google]]** (cross‑platform flexibility) as the *source of truth*.
- On an iPhone, add the chosen account under Settings → Accounts and enable only **Contacts** and **Calendars** for that account.
- Set the default contacts account to the chosen service to avoid accidental iCloud entries.
- Disable the competing service (e.g., turn off iCloud contacts/calendar sync) to stop duplicate databases.
- For photos, decide between **[[entities/icloud_photos]]** (tight native integration) and **[[entities/google_photos]]** (cross‑platform cloud storage). Both can serve as a *source of truth* for media, but the integration experience differs.

## Practical steps
1. **Select the ecosystem** – see [[concepts/ecosystem]] for criteria.
2. **Configure devices** – enable the chosen account on each device (iPhone, Windows laptop, tablet).
3. **Migrate existing data** – export from the old service (e.g., iCloud) and import into the new *source of truth* (Google) as described in the session.
4. **Turn off the old sync** – after verification, disable the previous service’s sync to prevent re‑adding data.

## Related concepts
- [[concepts/ecosystem]] – broader discussion of choosing iCloud vs. Google.
- [[concepts/mixing_and_matching]] – when and how to combine services without breaking the *source of truth*.
- [[concepts/smartwatch_integration]] – extending the *source of truth* to wearables (e.g., Fitbit, Garmin).

---
*This concept page synthesizes the recommendations from the conversation in [[summaries/session-38_2025-10-15]] and provides a reusable reference for managing a single authoritative data hub across devices.*