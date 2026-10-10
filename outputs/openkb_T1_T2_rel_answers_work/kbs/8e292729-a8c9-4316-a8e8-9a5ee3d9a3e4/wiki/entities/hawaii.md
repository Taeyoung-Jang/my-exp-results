---
sources: ["summaries/session-03_2025-06-15.md"]
type: "Place"
description: "U.S. state that does not observe daylight saving time"
---

# Hawaii

**Type:** Place

Hawaii is a U.S. state located in the Pacific Ocean that **does not observe [[concepts/daylight_saving_time]]**. Because it stays on a fixed offset year‑round, its local time can differ from the four continental U.S. zones ([[entities/pacific-time]], [[entities/mountain-time]], [[entities/central-time]], [[entities/eastern-time]]) during the months when those zones shift for DST.

- **Time‑zone offset:** Hawaii remains at UTC‑10, which is five hours behind Eastern Time and two hours behind Pacific Time when the latter is on standard time. See [[concepts/time_zone_offset]] for details on how offsets are expressed.
- **Reference handling:** When coordinating meetings across U.S. zones, Hawaii must be treated as a **non‑DST region**; schedules should explicitly note its constant offset. This is highlighted in [[summaries/session-03_2025-06-15]].
- **Related non‑DST region:** Like Hawaii, most of [[entities/arizona]] also does not observe DST, though it is in the Mountain Time region.

**Implications for scheduling:** Any meeting time anchored to a [[concepts/reference_time_zone]] (commonly Eastern Time) should include a separate conversion for Hawaii, because the usual one‑hour spacing between ET, CT, MT, and PT does not apply to Hawaii during DST periods.