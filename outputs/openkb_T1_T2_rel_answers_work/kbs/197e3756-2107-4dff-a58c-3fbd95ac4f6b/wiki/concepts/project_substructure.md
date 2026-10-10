---
type: "Concept"
sources: ["summaries/session-32_2025-02-13.md"]
description: "A minimal three‑folder layout inside each work project to keep docs, notes, and outputs separate."
---

# Project Substructure

**Definition**: A lightweight internal folder scheme for individual work projects that uses three subfolders—**Admin**, **Notes**, and **Outputs**—to separate contracts, meeting records, and final deliverables while staying easy to maintain.

## Origin
This structure originates from the discussion in [[summaries/session-32_2025-02-13]], where the user requested a simple yet functional layout for project files.

## Folder Layout
```
project‑<name>_YYYY/
├── Admin      # contracts, SOWs, amendments, administrative paperwork
├── Notes      # meeting notes, status reports, planning documents
└── Outputs    # final deliverables, reports, exported assets
```
- **Admin** holds any legally‑binding or logistical documents (e.g., `2026-02-10_sow_project-beta_signed.pdf`).
- **Notes** contains chronological notes and status updates (e.g., `2026-03-05_meeting-notes_project-beta.txt`).
- **Outputs** stores the finished work that is handed off to a client or stakeholder (e.g., `2026-04-20_final-deliverable_project-beta.pdf`).

## Why It Works
- **Simplicity**: Only three subfolders keep the hierarchy shallow, matching the broader [[concepts/folder_hierarchy]] guideline of limiting depth.
- **Consistency**: All files inside the project follow the same [[concepts/naming_conventions]] (`yyyy-mm-dd_description[_optional‑context].ext`), making them sortable and searchable.
- **Cross‑Device Friendly**: Folder names avoid spaces and special characters, aligning with [[concepts/cross_device_compatibility]] for seamless syncing between Windows and iPhone.

## Relationship to Other Concepts
- Ties into [[concepts/date_based_filenames]] because the naming pattern embeds dates, reinforcing chronological order without needing additional year subfolders.
- Complements the overall **Folder Hierarchy** approach, providing a clear, repeatable pattern for the *Work → Projects* branch.

## Practical Example
```
Work/
├── Projects/
│   └── project-beta_2026/
│       ├── Admin/
│       │   ├── 2026-02-10_sow_project-beta_signed.pdf
│       │   └── 2026-03-01_contract-amendment_project-beta.pdf
│       ├── Notes/
│       │   ├── 2026-03-05_meeting-notes_project-beta.txt
│       │   └── 2026-03-12_status-report_project-beta.docx
│       └── Outputs/
│           └── 2026-04-20_final-deliverable_project-beta.pdf
```

This layout provides enough structure to keep documents organized while remaining low‑maintenance.
