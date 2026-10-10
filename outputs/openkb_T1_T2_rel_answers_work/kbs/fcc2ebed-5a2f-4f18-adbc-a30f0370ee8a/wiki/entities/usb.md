---
sources: ["summaries/session-15_2025-06-15.md"]
type: "Product"
description: "Universal Serial Bus, a standard interface for connecting peripherals."
---

## USB (Universal Serial Bus)

USB is a widely used hardware interface that enables devices such as phones, cameras, and external drives to connect to a computer for data transfer and backup. In the context of the backup strategy discussed in [[summaries/session-15_2025-06-15]], USB serves as the primary method for importing phone photos to a computer without relying on cloud services.

Key points from the session:
- Used to connect phones (both [[entities/ios]] and [[entities/android]]) via a cable for manual photo imports.
- Works with the MTP protocol on Android devices, allowing the phone to appear as a camera or media device. [[entities/mtp]]
- Enables direct transfer to external drives that are part of the [[concepts/offline-backup]] and [[concepts/backup-redundancy]] setup.
- Provides a simple, low‑cost alternative to network‑based solutions such as a [[entities/nas]].

By leveraging USB connections, users can maintain a reliable and convenient backup workflow that emphasizes [[concepts/backup-reliability]] while keeping data offline.