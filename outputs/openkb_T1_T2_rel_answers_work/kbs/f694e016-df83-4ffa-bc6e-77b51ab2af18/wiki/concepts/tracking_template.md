---
type: "Concept"
sources: ["summaries/session-32_2024-12-16.md"]
description: "A TSV‑style sheet for tracking items, status, location, value, and actions during downsizing."
---

# Tracking Template

**Definition**: A simple, tab‑separated values (TSV) spreadsheet designed to capture every item in a downsizing project, its category, logistical details, and next steps. It is optimized for easy import into [[entities/google_sheets]] and supports quick weekly reviews.

## Core Columns
| Column | Purpose |
|--------|---------|
| **Item** | Brief description of the object (e.g., "Winter coat"). |
| **Category** | Decision outcome – `keep`, `sell`, `donate`, or `trash`. |
| **Listing Date** | Date the item was posted for sale (if applicable). |
| **Sell‑By Deadline** | Cut‑off date after which the item should be moved to donation. |
| **Final Status** | Result after the deadline – `sold`, `donated`, `packed`, etc. |
| **Location (Room)** | Physical location in the apartment (e.g., `kitchen`, `bedroom`). |
| **Estimated Value** | Approximate monetary value (useful for prioritising listings). |
| **Packed (Y/N)** | Marks whether the item has been placed in one of the two suitcases. |
| **Next action** | Immediate next step – `photograph`, `list`, `price drop`, `schedule pickup`, `donate drop‑off`, `pack`, or `none`. |
| **Notes** | Free‑form field for extra context (e.g., buyer communication). |

## How It Supports the [[concepts/downsizing_schedule]]
The template is referenced throughout the 16‑week, room‑based plan in [[summaries/session-32_2024-12-16]]. Each week’s tasks (e.g., admin weeks, catch‑up weeks) correspond to updates in the **Next action** column, ensuring that the workload stays within the [[concepts/time_budgeting]] limit of 3–5 hours.

## Review Routine
A recommended habit is a **twice‑weekly review** (see [[concepts/review_routine]]):
1. **Start‑of‑week** – scan the sheet, set priority items, and assign concrete next actions.
2. **End‑of‑week** – update statuses, check any `Sell‑By Deadline` that has passed, and move stalled items to donation.

This lightweight check‑in takes only a few minutes and keeps the downsizing flow on track.

## Integration with Other Concepts
- **[[concepts/admin_weeks]]**: During admin weeks, the sheet is populated with photographs, listings, and pricing details.
- **[[concepts/catch_up_weeks]]** and **[[concepts/buffer_zone]]**: The template highlights lagging items, making it easy to allocate catch‑up time.
- **[[concepts/room_based_planning]]**: Items are filtered by `Location (Room)` to focus weekly effort on a specific area.
- **[[concepts/sentimental_decluttering]]**: Sentimental items are flagged with `keep` and `Packed (Y/N)` to track what ultimately makes it into the suitcases.

## Practical Tips
- Copy the TSV block below into a new Google Sheet; the platform will automatically split columns.
- Keep the **Estimated Value** column modest – it’s for prioritisation, not appraisal.
- Use conditional formatting in Google Sheets to highlight rows past their `Sell‑By Deadline`.

```tsv
Item	Category	Listing Date	Sell-By Deadline	Final Status	Location (Room)	Estimated Value	Packed (Y/N)	Next action	Notes
Winter coat	sell	2026-01-10	2026-01-24	donated	bedroom	40	N	drop off	No buyer interest
Old blender	donate				donated	kitchen	0	N	none	Drop-off Week 7
Photo album	keep				living room	0	Y	none	Packed in suitcase A
Bookshelf	sell	2026-02-02	2026-02-16	sold	living room	60	N	schedule pickup	Pickup completed
Ceramic mugs	donate				donated	kitchen	0	N	none	Bundled with kitchenware
Beloved sweater	keep				bedroom	20	Y	pack	Suitcase B essential
Travel adapter	keep				office	10	Y	pack	Going in front pocket
```

---
*This concept page captures the structure, purpose, and operational integration of the tracking template used in the downsizing plan.*