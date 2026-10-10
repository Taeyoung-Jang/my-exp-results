---
type: "Concept"
sources: ["summaries/session-32_2024-12-13.md"]
description: "Standardized naming for travel photo folders to aid organization and backup."
---

# Trip Folder Naming

## Definition
**Trip Folder Naming** is a consistent convention for naming directories that store photos and videos from a specific travel event. The convention typically includes the year, month, and a brief location descriptor (e.g., `2025-02 Japan`).

## Rationale
A predictable folder name makes it easy to locate, sort, and back up media later. When combined with an [[concepts/incoming-folder]] and automated backup tools, the naming scheme enables a smooth, low‑effort workflow that reduces the chance of duplicate archives and simplifies recovery.

## Recommended Pattern
```
YYYY-MM <Location>
```
- **YYYY** – Four‑digit year of the trip.
- **MM** – Two‑digit month.
- **Location** – Short, human‑readable place name (city, country, or region).

_Example_: `2025-02 Japan`

## Implementation Steps (derived from [[summaries/session-32_2024-12-13]])
1. After dumping new media into the **Photos Incoming** folder, perform a quick [[concepts/duplicate-removal]] pass.
2. Create a new folder using the naming pattern above.
3. Move the cleaned files into this folder.
4. Ensure the folder resides within the main photo archive that is covered by [[concepts/cloud-backup]] and [[concepts/external-drive-mirroring]].
5. The next time the external drive is connected, your [[concepts/plug-and-forget-backup]] solution (e.g., Windows File History) will automatically sync the new trip folder.

## Benefits
- **Searchability** – Enables chronological sorting and quick filtering by location.
- **Backup Consistency** – Guarantees that backup tools recognize the folder as part of the primary archive.
- **Scalability** – Works regardless of how many trips you accumulate over years.

## Related Concepts
- [[concepts/incoming-folder]]
- [[concepts/cloud-backup]]
- [[concepts/duplicate-removal]]
- [[concepts/external-drive-mirroring]]
- [[concepts/plug-and-forget-backup]]

---
*This concept is illustrated in [[summaries/session-32_2024-12-13]].*