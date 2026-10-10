---
type: "Concept"
sources: ["summaries/session-32_2025-02-13.md"]
description: "Using year‑based subfolders for high‑volume personal finance documents."
---

## Year Subfolders

**Definition**: A selective folder structure where certain categories (e.g., Taxes and Insurance) are further divided by calendar year to manage large volumes of documents while still relying on a consistent naming scheme.

**Key Details from [[summaries/session-32_2025-02-13]]**:
- Applied only to *Personal → Documents → Finance → Taxes* and *Insurance*.
- Receipts remain in a flat folder; the year‑based hierarchy is optional and used where files accumulate rapidly.
- The approach pairs with the overall *folder_hierarchy* and *naming_conventions* strategy, keeping the system shallow (max 2‑3 levels) while still providing chronological ordering.

**Why Use Year Subfolders?**
- **Scalability**: As tax returns and insurance policies grow each year, a separate `2025`, `2026`, … folder prevents a single directory from becoming unwieldy.
- **Searchability**: Combined with the `yyyy-mm-dd_description.ext` *date_based_filenames* pattern, users can locate files via date or by browsing the year folder.
- **Low Maintenance**: Only two categories employ year subfolders, so the majority of personal files stay flat, preserving the minimal‑maintenance ethos.
- **Cross‑Device Compatibility**: Folder names contain only alphanumeric characters and dashes, ensuring seamless syncing between Windows and iPhone devices.

**Implementation Guidelines**
1. Create top‑level folders `Taxes` and `Insurance` under `Personal/Documents/Finance`.
2. Inside each, add year subfolders (e.g., `2025`, `2026`).
3. Store files using the unified naming pattern: `yyyy-mm-dd_description.ext`.
4. Keep `Receipts` flat; rely on the date in the filename for chronological sorting.

**Related Concepts**
- [[concepts/folder_hierarchy]] – overall shallow structure the year subfolders extend.
- [[concepts/naming_conventions]] – the date‑centric filename format that works hand‑in‑hand with year folders.
- [[concepts/date_based_filenames]] – ensures files sort correctly both within and across year folders.
- [[concepts/cross_device_compatibility]] – guarantees the folder scheme works on Windows and iPhone.
