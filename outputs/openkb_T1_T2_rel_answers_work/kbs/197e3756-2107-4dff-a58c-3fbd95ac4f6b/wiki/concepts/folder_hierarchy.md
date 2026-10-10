---
type: "Concept"
sources: ["summaries/session-32_2025-02-13.md"]
description: "A shallow two‑level folder layout that separates personal and work files for easy sync and maintenance."
---

# Folder Hierarchy

**Definition**: A shallow, two‑level directory structure that separates personal and work data into distinct top‑level folders, each containing a small set of broad categories. The design prioritises simplicity, cross‑device compatibility, and low maintenance.

---

## Core Structure

The hierarchy advocated in [[summaries/session-32_2025-02-13]] consists of two primary top‑level directories:

```
Personal
Work
```

### Personal

- **Documents** – Sub‑folders for Finance (Taxes, Insurance, Receipts), Identity, Health, Home.
- **Photos** – Light sub‑folders such as Family, Trips, Misc.
- **Archive** – Long‑term storage for completed or older items.

### Work

- **Documents** – Sub‑folders for Contracts, HR, Admin, Reference.
- **Projects** – Contains one folder per active project, each with a minimal internal layout (see [[concepts/project_substructure]]).
- **Archive** – Stores finished projects and deprecated material.

The hierarchy intentionally avoids deep nesting (no more than two levels beneath the top‑level category) to keep the system easy to navigate on both Windows and iPhone devices.

---

## Why a Shallow Hierarchy?

1. **Ease of Use** – Fewer clicks to reach any file, encouraging consistent use.
2. **Sync‑Friendliness** – Simple paths reduce the risk of sync conflicts across platforms like Windows 11 and iPhone.
3. **Searchability** – Coupled with a consistent [[concepts/naming_conventions]] and [[concepts/date_based_filenames]] pattern, files can be located via search rather than deep folder navigation.
4. **Scalability** – Adding new categories or projects requires only a new top‑level folder or a single sub‑folder, preserving the overall simplicity.

---

## Interaction with Other Concepts

- **[[concepts/naming_conventions]]** – The folder hierarchy works hand‑in‑hand with a uniform naming scheme to make files sortable and searchable without needing deep folder paths.
- **[[concepts/date_based_filenames]]** – Relying on date‑prefixed filenames reduces the need for additional chronological sub‑folders, allowing the hierarchy to stay flat.
- **[[concepts/year_subfolders]]** – An exception to the flat approach: year sub‑folders are used only for high‑volume categories like Taxes and Insurance within the Personal → Documents → Finance branch.
- **[[concepts/project_substructure]]** – Within each Work → Projects folder, a minimal three‑folder layout (Admin, Notes, Outputs) maintains order without deep nesting.
- **[[concepts/cross_device_compatibility]]** – By avoiding spaces and special characters in folder names, the hierarchy ensures seamless syncing between Windows 11 and iPhone devices.

---

## Implementation Tips

- **Consistency** – Use the exact folder names as defined; avoid ad‑hoc variations.
- **Naming** – Pair the hierarchy with the `yyyy-mm-dd_description.ext` pattern to keep sorting logical.
- **Archiving** – Periodically move completed items into the appropriate Archive folder to keep active directories tidy.
- **Backup** – Complement the hierarchy with a regular local backup strategy (see [[concepts/local_backup_strategy]]) to protect against data loss.

---

## Example Path

```
Personal/Documents/Finance/Taxes/2025/2025-04-15_tax-return.pdf
Work/Projects/project-beta_2026/Outputs/2026-04-20_final-deliverable_project-beta.pdf
```