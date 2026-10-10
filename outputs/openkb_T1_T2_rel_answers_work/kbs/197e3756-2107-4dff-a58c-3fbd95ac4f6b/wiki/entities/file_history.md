---
sources: ["summaries/session-32_2025-02-13.md", "summaries/session-12_2024-06-15.md"]
type: "Product"
description: "File History is a Windows 11 product for automatic versioned backups of user folders."
---

## File History

File History is a **product** bundled with Windows 11 that provides automatic, versioned backup of selected user folders to an external drive. In the conversation **[[summaries/session-12_2024-06-15]]**, the assistant recommends using File History as the simplest built‑in way to achieve a weekly, local‑only backup routine.

### Key facts from the sessions
- **Purpose:** Continuously backs up user data (Documents, Pictures, Videos, Desktop, custom Projects folder) without requiring a full system image.
- **Setup steps** (as outlined in the session):
  1. Open **Control Panel → System and Security → File History**.
  2. Turn on File History and select the external drive.
  3. Use **Advanced settings** to add the custom **Projects** folder.
  4. Set backup frequency to **Daily** (runs when the drive is connected) and retention to **"Until space is needed"**.
- **Automation:** Works automatically whenever the designated external drive is plugged in, fitting the weekly plug‑in routine described.
- **Scope:** Targets only user folders, aligning with the advice to avoid full system‑image backups for a lightweight solution.
- **Integration with proposed folder hierarchy:** The shallow, two‑level folder structure and date‑centric naming pattern recommended in **[[summaries/session-32_2025-02-13]]** (see [[concepts/folder_hierarchy]] and [[concepts/naming_conventions]]) complement File History. Because folders are not deeply nested and filenames follow a consistent `yyyy-mm-dd_description` format, versioned restores are easy to locate and manage.
- **Cross‑device considerations:** While File History handles local versioning, the same folder layout works well with cloud or device syncing (e.g., between Windows and iPhone) as described in [[concepts/cross_device_compatibility]]. Using the same naming conventions ensures that synced copies retain searchable, sortable names.
- **Year subfolders:** For high‑volume categories like Taxes and Insurance, the suggested year‑based subfolders (see [[concepts/year_subfolders]]) coexist smoothly with File History, as the backup engine tracks changes regardless of additional sub‑levels.

### Related concepts
- [[concepts/folder_hierarchy]] – the simple top‑level Personal/Work layout monitored by File History.
- [[concepts/naming_conventions]] – the consistent `yyyy-mm-dd_description` pattern that aids versioning.
- [[concepts/date_based_filenames]] – improves sorting and retrieval of backed‑up files.
- [[concepts/local_backup_strategy]] – the broader strategy of rotating external drives and weekly backups.
- [[concepts/cross_device_compatibility]] – ensures the folder structure works across Windows and iPhone.
- [[concepts/year_subfolders]] – optional year folders for finance docs that File History handles seamlessly.

### Related entities
- [[entities/windows_11]] – the operating system that includes File History.
- [[entities/microsoft]] – the company that develops Windows 11 and File History.