---
type: "Concept"
sources: ["summaries/session-32_2025-02-13.md"]
description: "Ensuring file organization works seamlessly across Windows and iPhone devices."
---

# Cross‑Device Compatibility

## Overview
Cross‑Device Compatibility is the practice of designing folder structures and naming conventions that function reliably on multiple platforms—specifically Windows PCs and iOS devices. By avoiding spaces, using only lowercase letters, dashes, and underscores, and relying on a consistent date‑based pattern, files remain sortable, searchable, and sync‑friendly across different operating systems.

## Key Principles from [[summaries/session-32_2025-02-13]]
- **Folder hierarchy**: A shallow two‑level tree (Personal / Work) that mirrors on both platforms, reducing path‑length issues. [[concepts/folder_hierarchy]]
- **Naming conventions**: `yyyy-mm-dd_description[_optional‑context].ext` using lowercase and dashes; this format is safe for Windows file systems and iOS file browsers. [[concepts/naming_conventions]]
- **Date‑based filenames**: Enables chronological sorting without extra subfolders, which is especially useful when syncing. [[concepts/date_based_filenames]]
- **Selective year subfolders**: Applied only to high‑volume finance categories (Taxes, Insurance) to keep the flat structure manageable while still supporting quick navigation. [[concepts/year_subfolders]]
- **Project substructure**: A minimal three‑folder layout (Admin, Notes, Outputs) inside each project folder, keeping work files organized without adding complexity. [[concepts/project_substructure]]

## Platform‑Specific Considerations
- **Windows 11**: Avoid reserved characters (`<>:"/\|?*`) and keep path lengths under the OS limit. The chosen naming scheme complies with these constraints. [[entities/windows_11]]
- **iPhone (iOS)**: The Files app displays filenames exactly as stored; using dashes and underscores ensures readability and prevents automatic URL‑encoding. [[entities/iPhone]]
- **Microsoft ecosystem**: When using OneDrive or SharePoint for syncing, the same conventions prevent conflicts and preserve file history. [[entities/microsoft]]

## Interaction with Syncing and History
Consistent naming and a predictable folder layout improve the reliability of automatic syncing services (e.g., OneDrive, iCloud) and make it easier to trace file changes via version history. [[entities/file_syncing]]

## Related Concepts
- [[concepts/folder_hierarchy]]
- [[concepts/naming_conventions]]
- [[concepts/date_based_filenames]]
- [[concepts/year_subfolders]]
- [[concepts/project_substructure]]
- [[entities/file_history]]

---
*This concept page synthesizes the recommendations from the conversation in [[summaries/session-32_2025-02-13]] to provide a reusable reference for building cross‑device compatible file systems.*