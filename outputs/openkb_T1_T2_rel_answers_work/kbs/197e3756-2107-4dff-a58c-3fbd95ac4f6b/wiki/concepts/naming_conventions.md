---
type: "Concept"
sources: ["summaries/session-32_2025-02-13.md"]
description: "Standardized file naming patterns for cross‑device, searchable organization."
---

# Naming Conventions

**Type:** Concept
**Description:** A consistent, Windows‑safe pattern for naming files that supports easy searching, chronological sorting, and seamless syncing across devices.

---

## Core Pattern
The recommended filename format introduced in [[summaries/session-32_2025-02-13]] is:

```
yyyy-mm-dd_description_optional‑context.ext
```

- **yyyy‑mm‑dd** – Four‑digit year, two‑digit month, two‑digit day. Provides natural chronological ordering.
- **description** – Brief, lower‑case, dash‑separated keywords that surface the file’s purpose.
- **optional‑context** – Project name, client, or other qualifier when useful.
- **ext** – Standard file extension (pdf, jpg, docx, etc.).

### Rules of Thumb
1. **Lowercase & Dashes** – Avoid spaces and capital letters to stay Windows‑compatible and iPhone‑friendly.
2. **Date First** – Placing the date at the start ensures files sort by creation/occurrence date in any file explorer.
3. **Keyword Priority** – Put the most important searchable terms at the beginning of the description.
4. **Versioning** – Append `v1`, `v2`, … before the extension for iterative drafts (e.g., `2026-03-05_meeting-notes_project‑beta_v2.txt`).
5. **Non‑Date Files** – When a file isn’t tied to a specific date, start with the primary keyword and optionally add a date later (e.g., `contract_client‑alpha.pdf`).

---

## Benefits
- **Cross‑device compatibility** – Works on both Windows and iPhone, aligning with [[concepts/cross_device_compatibility]].
- **Searchability** – Consistent keywords and date prefixes make built‑in OS search tools highly effective.
- **Minimal Maintenance** – A single pattern reduces decision fatigue and eliminates the need for extensive folder nesting, complementing the [[concepts/folder_hierarchy]] approach.
- **Scalability** – Works for personal documents, photos, and work‑related assets alike.

---

## Examples from Session 32
| Context | Filename Example |
|---------|-----------------|
| Tax receipt | `2025-02-14_tax-receipt_home-office.pdf` |
| Contract | `2026-01-05_contract_client-alpha.pdf` |
| Meeting notes | `2026-03-12_meeting-notes_project-beta.txt` |
| Photo | `2025-07-18_family-picnic.jpg` |
| Scan | `scan_passport_2026-renewal.pdf` |

---

## Related Concepts
- [[concepts/date_based_filenames]] – Emphasizes the importance of embedding dates in file names.
- [[concepts/folder_hierarchy]] – Shows how naming conventions reduce the need for deep folder structures.
- [[concepts/project_substructure]] – Works together with naming conventions to keep project files organized.
- [[concepts/year_subfolders]] – A complementary strategy for high‑volume categories like Taxes and Insurance.

---

## Implementation Tips
1. **Create a cheat‑sheet** of the pattern and keep it in a visible location (e.g., a README in the top‑level folder).
2. **Automate where possible** – Use OS automation scripts or third‑party tools to prepend dates to new files.
3. **Educate collaborators** – Share the convention with teammates to maintain consistency across shared workspaces.

---

*Page created based on the guidance from [[summaries/session-32_2025-02-13]].*