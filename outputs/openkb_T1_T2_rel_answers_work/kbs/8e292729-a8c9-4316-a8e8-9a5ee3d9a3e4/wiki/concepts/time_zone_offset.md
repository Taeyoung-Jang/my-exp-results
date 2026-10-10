---
type: "Concept"
sources: ["summaries/session-03_2025-06-15.md"]
description: "Difference in clock time between geographical time zones."
---

# Time Zone Offset

**Definition**: A time zone offset is the fixed number of hours (and sometimes minutes) that a particular region's local time differs from a reference time, typically Coordinated Universal Time (UTC) or another chosen reference zone.

## Key Details
- In the United States, the four main continental zones form a simple one‑hour step chain: Pacific Time is three hours behind Eastern Time, Mountain Time two hours behind, and Central Time one hour behind.  
- The document [[summaries/session-03_2025-06-15]] uses **Eastern Time** as the reference zone and shows example conversions:
  - 10:00 AM ET → 9:00 AM CT → 8:00 AM MT → 7:00 AM PT
  - 3:00 PM ET → 2:00 PM CT → 1:00 PM MT → 12:00 PM PT
- Offsets remain constant across daylight‑saving transitions for the four main zones because they all shift simultaneously.
- Exceptions occur in regions that do not observe daylight saving, such as **Arizona** (Mountain Time without DST) and **Hawaii** (its own zone), where the offset relative to the reference zone changes during the DST period.

## Related Concepts
- [[concepts/reference_time_zone]] – Choosing a single zone as the anchor for all scheduling.
- [[concepts/daylight_saving_time]] – How DST impacts (or does not impact) offsets.
- [[concepts/time_zone_offset]] – This concept itself, describing the systematic hour differences.

## Entities Involved
- [[entities/eastern-time]] – Reference zone in the example.
- [[entities/central-time]] – One‑hour offset from ET.
- [[entities/mountain-time]] – Two‑hour offset from ET.
- [[entities/pacific-time]] – Three‑hour offset from ET.
- [[entities/arizona]] – Example of a non‑DST region affecting offset.
- [[entities/hawaii]] – Another non‑DST region.
