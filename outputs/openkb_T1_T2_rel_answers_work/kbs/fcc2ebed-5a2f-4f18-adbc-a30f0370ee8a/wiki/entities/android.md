---
sources: ["summaries/session-32_2025-09-12.md", "summaries/session-15_2025-06-15.md"]
type: "Product"
description: "Android is a mobile operating system used on many smartphones and tablets."
---

# Android (product)

Android is a widely used mobile operating system developed by Google, powering a large variety of smartphones and tablets.

## Role in the backup discussion
In the conversation documented in [[summaries/session-15_2025-06-15]], Android devices were referenced as a source of photos that need to be backed up without using cloud services. The recommended workflow involves connecting the Android phone to a computer via **USB** and using the **MTP** (Media Transfer Protocol) to transfer images to a local folder structure that participates in an **offline backup** strategy.

Key points highlighted:
- Use a USB connection (often appearing as an MTP device) to import photos directly to the computer. [[entities/usb]] [[entities/mtp]]
- Store the imported photos in a designated folder that is included in the regular backup routine, supporting [[concepts/backup-reliability]] and [[concepts/backup-redundancy]].
- This approach aligns with an [[concepts/offline-backup]] model that avoids reliance on cloud sync.

## Related concepts and entities
- [[concepts/backup-reliability]] – ensuring the backup process runs automatically and without manual effort.
- [[concepts/backup-redundancy]] – keeping multiple copies in separate physical locations.
- [[concepts/offline-backup]] – a backup strategy that does not depend on internet services.
- [[entities/nas]] – mentioned as an optional alternative for central storage, though not required for the Android workflow.

For the full context of this recommendation, see the session summary: [[summaries/session-15_2025-06-15]].

See also: [[summaries/session-32_2025-09-12]]