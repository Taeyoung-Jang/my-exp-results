---
sources: ["summaries/session-38_2025-10-15.md"]
type: "Product"
description: "Google Photos is Google's cloud photo storage and backup service."
---

# Google Photos

Google Photos is a cloud‑based photo storage and backup service provided by [[entities/google]]. It offers automatic backup, powerful search, and cross‑platform access.

## Key facts from [[summaries/session-38_2025-10-15]]
- **Cross‑platform sync**: Recommended as the central photo library for users who move between iPhone, Windows laptop, and other devices, fitting the [[concepts/cross_platform_sync]] approach.
- **Integration on iPhone**: Works on iOS but does **not** integrate into the native Photos app, resulting in a separate local camera‑roll library until the app uploads images.
- **Duplicate avoidance**: Because iCloud Photos remains active, users may end up with two libraries; turning off iCloud syncing for photos is advised to follow the [[concepts/duplicate_avoidance]] principle.
- **Trade‑offs vs. iCloud Photos**: 
  - No seamless handling of Live Photos or original‑resolution files like [[entities/icloud_photos]] provides.
  - Slight differences in processing and metadata handling.
  - Still offers excellent search, reliability, and cross‑device availability.
- **Source of truth**: When used as the primary photo store, Google Photos becomes the [[concepts/source_of_truth]] for images across devices.

## Role in an ecosystem
Google Photos fits within a broader [[concepts/ecosystem]] strategy where a single service acts as the master repository for a data type (photos, in this case). By aligning all devices to upload to Google Photos, users maintain consistency with minimal manual effort.

## Related concepts and entities
- [[concepts/source_of_truth]]
- [[concepts/duplicate_avoidance]]
- [[concepts/cross_platform_sync]]
- [[concepts/ecosystem]]
- [[entities/icloud_photos]] (for comparison)
- [[entities/iphone]] (platform where integration nuances appear)
- [[entities/windows]] (platform that accesses Google Photos via web or apps)
