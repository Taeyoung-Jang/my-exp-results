---
sources: ["summaries/session-15_2025-06-15.md"]
type: "Other"
description: "MTP is a protocol for transferring files between computers and mobile devices over USB."
---

# MTP (Media Transfer Protocol)

**Type:** other

## What it is
MTP (Media Transfer Protocol) is a standard protocol used to transfer media files—such as photos, videos, and documents—between a computer and a mobile device over a USB connection. It is commonly employed by Android phones and other devices that present themselves as portable media players when plugged in.

## Role in the backup workflow (session‑15_2025‑06‑15)
- In the discussed backup strategy, MTP is mentioned as a way to mount an Android device for **offline‑backup** of photos without using any cloud services.  
- The assistant recommends using MTP (or the equivalent USB mass‑storage mode on iOS) to copy new photos to a designated folder on the computer, which is then captured by the two‑drive backup system.
- This method supports the principles of **backup‑reliability** and **backup‑redundancy** by ensuring that a local copy of phone photos is regularly imported and protected on encrypted external drives.

## Related concepts
- [[concepts/offline-backup]] – the overall strategy of keeping backups local and not reliant on cloud services.
- [[concepts/backup-reliability]] – emphasizing automatic, hands‑off operations like MTP‑based imports.
- [[concepts/backup-redundancy]] – duplicating the imported photos across multiple external drives.

## Related entities
- [[entities/android]] – a common platform that uses MTP for file transfers.
- [[entities/ios]] – while iOS does not natively use MTP, similar USB transfer methods apply.
- [[entities/usb]] – the physical interface through which MTP operates.
- [[entities/nas]] – mentioned as an optional alternative to the two‑drive approach.

## Source reference
- This information is drawn from the discussion in [[summaries/session-15_2025-06-15]], where MTP is recommended for importing phone photos into the local backup folder structure.