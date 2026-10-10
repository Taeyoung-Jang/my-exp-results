---
sources: ["summaries/session-32_2025-02-13.md"]
type: "Product"
description: "A cross‑device service that keeps files synchronized automatically."
---

## Automatic File Syncing

**Type:** product

Automatic File Syncing is the background service the user set up to keep documents and photos up‑to‑date across all of their devices, including Windows 11 computers and an iPhone.  The service underpins the file‑organization recommendations discussed in [[summaries/session-32_2025-02-13]], allowing the user to rely on a single, consistent folder hierarchy without manually copying files.

### Key Facts from the Session
- **Cross‑device compatibility:** The syncing works between Windows 11 and iPhone, making the proposed naming conventions and folder layout usable on both platforms.  This aligns with the [[concepts/cross_device_compatibility]] concept.
- **Support for naming conventions:** By keeping filenames in a uniform `yyyy-mm-dd_description.ext` format, the sync service can resolve conflicts more reliably, reflecting the [[concepts/naming_conventions]] and [[concepts/date_based_filenames]] ideas.
- **Low‑maintenance structure:** The recommended shallow [[concepts/folder_hierarchy]] (Personal / Work) and selective year subfolders rely on the sync service to propagate changes instantly, reducing the need for manual backups.
- **Interaction with other entities:** The service ties directly to the user’s **Windows 11** system and their **iPhone**, ensuring seamless synchronization across both ecosystems.

### Related Entities and Concepts
- [[entities/windows_11]] – the primary desktop OS where the sync client runs.
- [[entities/iPhone]] – the mobile device receiving synchronized files.
- [[concepts/cross_device_compatibility]] – the principle of making files accessible on multiple platforms.
- [[concepts/folder_hierarchy]] – the suggested top‑level Personal/Work structure.
- [[concepts/naming_conventions]] – the consistent filename pattern that aids syncing.
- [[concepts/date_based_filenames]] – ensures chronological ordering across devices.

### Relevance
Automatic File Syncing is the foundational technology that enables the user’s streamlined file‑organization system, making the recommendations from the session practical and reliable.
