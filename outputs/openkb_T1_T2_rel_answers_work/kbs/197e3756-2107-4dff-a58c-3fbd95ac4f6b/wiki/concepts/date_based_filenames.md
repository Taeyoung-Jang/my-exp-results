---
type: "Concept"
sources: ["summaries/session-32_2025-02-13.md"]
description: "A filename scheme using YYYY‑MM‑DD and descriptive text for easy sorting and searching."
---

## Date‑Based Filenames

**Definition**: A naming pattern that starts with a date in the form `yyyy-mm-dd` followed by a concise, hyphen‑separated description, optionally ending with project or client identifiers. It is designed to be lowercase, Windows‑safe, and searchable across devices.

### Overview
Date‑based filenames provide chronological ordering automatically when files are listed alphabetically. By embedding the date at the start, users can locate files by time period without needing additional folder layers.

### Pattern
```
yyyy-mm-dd_description_optional‑context.ext
```
- **yyyy‑mm‑dd** – Four‑digit year, two‑digit month, two‑digit day.
- **description** – Key terms describing the content, placed early for quick scanning.
- **optional‑context** – Project name, client, or other identifier when relevant.
- Use **lowercase**, **dashes**, and avoid spaces to ensure compatibility with Windows and iPhone.

### Benefits
- **Chronological sorting** without extra folders.
- **Cross‑device compatibility**: works on Windows, iPhone, and cloud syncing services. [[concepts/cross_device_compatibility]]
- **Searchability**: keyword appears early, improving results in OS search tools.
- **Consistency**: aligns with broader naming guidelines. [[concepts/naming_conventions]]

### Example Filenames from Session 32
- `2026-01-15_tax-return.pdf`
- `2026-02-03_receipt_laptop-purchase.pdf`
- `2026-03-12_contract_client-alpha.pdf`
- `2026-03-10_meeting-notes_project-beta.txt`
- `2025-07-18_family-picnic.jpg`
- `scan_passport_2026-renewal.pdf` (non‑date file, keyword first)

### Implementation Guidance
1. **Adopt the pattern** for all new files across Personal and Work domains.
2. **Retrofit** existing high‑volume categories (e.g., Finance → Taxes, Insurance) by renaming files to the pattern; keep the folder hierarchy shallow. [[concepts/folder_hierarchy]]
3. **Integrate with project subfolders**: use the same pattern inside `Admin`, `Notes`, and `Outputs` to keep contracts, meeting notes, and deliverables distinct yet uniformly named. [[concepts/project_substructure]]
4. **Year subfolders** are optional; date‑based names often make them unnecessary, but they can still be used for very large collections such as Taxes and Insurance. [[concepts/year_subfolders]]

### Related Concepts
- [[concepts/naming_conventions]]
- [[concepts/folder_hierarchy]]
- [[concepts/cross_device_compatibility]]
- [[concepts/project_substructure]]
- [[concepts/year_subfolders]]

### Source
This concept is derived from the discussion in [[summaries/session-32_2025-02-13]], where a unified filename scheme was recommended for both personal and work files.