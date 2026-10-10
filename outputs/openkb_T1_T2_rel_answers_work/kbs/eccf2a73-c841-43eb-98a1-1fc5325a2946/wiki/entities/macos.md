---
sources: ["summaries/session-12_2024-06-15.md"]
type: "Product"
description: "Apple's desktop operating system for Mac computers."
---

# macOS (product)

macOS is the desktop operating system developed by Apple Inc. for its line of Mac computers. In the context of **session-12_2024-06-15**, macOS serves as the platform on which the user implements backup strategies for cloud‑based data.

## Key points from the session
- The user is on a **Mac**, so all recommended tools (e.g., [[entities/time-machine]], [[entities/carbon-copy-cloner]], and [[entities/chronosync]]) are macOS applications.
- macOS can keep cloud files locally synced, enabling one‑way backup workflows that rely on the OS’s file system APIs.
- The OS supports built‑in versioned backups via **Time Machine**, but the session notes that Time Machine works best only when cloud files are fully downloaded to the local drive.
- For more granular control, macOS users can employ third‑party one‑way backup tools such as Carbon Copy Cloner and ChronoSync, both of which integrate tightly with the macOS file system.
- Handling of “online‑only” cloud files on macOS requires either marking folders as *always keep on this device* within the cloud client or manually downloading them before backup.

## Related concepts and entities
- [[concepts/cloud-storage-vs-external-drive]] – the decision framework discussed for choosing between cloud and external drives.
- [[concepts/one-way-backup]] – the recommended backup mode to avoid reverse syncing.
- [[concepts/online-only-file-handling]] – strategies for dealing with placeholder files that exist only in the cloud.
- [[entities/time-machine]] – Apple’s native backup utility that runs on macOS.
- [[entities/carbon-copy-cloner]] – third‑party macOS app for one‑way copy tasks with safety nets.
- [[entities/chronosync]] – another macOS backup/sync tool supporting left‑to‑right backups.

## Source
- Summarized in [[summaries/session-12_2024-06-15]].