---
type: "Concept"
sources: ["summaries/session-10_2025-06-15.md"]
description: "Guidelines for consistent folder and file naming to aid sorting and retrieval"
---

# Naming Conventions

## Overview
Naming conventions are systematic rules for constructing folder and file names so that items can be located quickly, sorted chronologically, and understood at a glance. Consistent naming reduces ambiguity and prevents duplicate structures.

## Core pattern from [[summaries/session-10_2025-06-15]]
- **Folder names**: `ProjectName_YYYY‑MM` (e.g., `ClientA_ProjectAlpha_2026-03`).
- **File names**: `Category_Description_YYYY‑MM‑DD` (e.g., `Report_Summary_2026-03-17`).
- Use underscores or hyphens as separators; avoid spaces for better cross‑platform compatibility.

## Benefits
- Immediate temporal context without opening the file.
- Easy lexical sorting aligns with chronological order.
- Uniformity across [[entities/work]], [[entities/personal]], [[entities/finances]], [[entities/media]], [[entities/reference]], and [[entities/apps_utilities]] folders.

## Relationship to other concepts
- Works hand‑in‑hand with the **folder hierarchy** defined in [[concepts/folder_hierarchy]] to give each top‑level bucket a clear, predictable internal structure.
- Supports the **inbox management** workflow from [[concepts/inbox_management]] by providing a ready destination name for each newly sorted item.

## Example tree (2–3 levels deep) demonstrating naming conventions
```
Work
 Projects
  ClientA_ProjectAlpha_2026-03
   Report_Summary_2026-03-17.docx
  ClientB_AppRedesign_2025-11
   Specs_Design_2025-11-02.pdf
Personal
 Travel
  Trip_Paris_2024-07
   Itinerary_2024-07-01.pdf
Finances
 Taxes
  TaxReturn_2023-04.pdf
Media
 Photos
  Vacation_2023-06-15.jpg
``` 

## Implementation tips
1. **Start with a template**: create a short cheat‑sheet with the patterns above.
2. **Automate where possible**: use OS scripting or file‑renaming tools to apply the format.
3. **Apply consistently**: enforce the rule when moving items from the inbox or when creating new documents.
4. **Review periodically**: ensure the date format matches your regional preferences (ISO 8601 `YYYY‑MM‑DD` is recommended).

By adopting these naming conventions, you create a self‑documenting file system that scales without growing chaotic.