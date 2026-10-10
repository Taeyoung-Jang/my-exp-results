---
sources: ["summaries/session-38_2025-10-15.md"]
type: "Product"
description: "Apple's flagship smartphone, central to cross‑platform sync strategies."
---

# iPhone

**Product** – The iPhone is Apple’s flagship smartphone, frequently used as a primary device in multi‑device workflows.

### Role in Cross‑Platform Sync
- In the context of [[summaries/session-38_2025-10-15]], the iPhone is configured to use [[entities/google]] as the **[[concepts/source_of_truth]]** for contacts and calendars.
- Users are advised to add their Google account in **Settings → Accounts**, enable only **Contacts** and **Calendars**, and set Google as the default contacts account. This prevents duplicate data arising from simultaneous [[entities/icloud]] sync, addressing [[concepts/duplicate_avoidance]].
- The iPhone can still participate in a broader [[concepts/cross_platform_sync]] strategy that includes a [[entities/windows]] laptop and other devices.

### Photo Management
- When using [[entities/google_photos]] on the iPhone, photos first reside in the local camera roll before being uploaded, creating a separate local library from the cloud.
- By contrast, [[entities/icloud_photos]] integrates directly with the native **Photos** app, offering seamless handling of Live Photos and original‑resolution files.
- The choice between these services reflects the trade‑off between tight ecosystem integration (iCloud) and cross‑platform flexibility (Google).

### Ecosystem Considerations
- The iPhone exemplifies the [[concepts/ecosystem]] approach of selecting a single **source of truth** (Google or iCloud) and disabling competing sync services to maintain data consistency.
- This aligns with the recommendations in the session summary to avoid mixing and matching sync sources unless a specific feature gap exists.

### Related Entities
- Manufacturer: [[entities/apple]]
- Competing platforms mentioned: [[entities/samsung]]
- Sync services: [[entities/google]], [[entities/icloud]]
- Photo services: [[entities/google_photos]], [[entities/icloud_photos]]

---
*Referenced in [[summaries/session-38_2025-10-15]]*