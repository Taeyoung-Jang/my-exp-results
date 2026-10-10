---
sources: ["summaries/session-02_2024-06-15.md"]
type: "Product"
description: "Apple's cloud storage and sync service for devices and apps."
---

# iCloud

**Type:** Product

**Owner:** [[entities/apple]]

## Overview
iCloud is Apple’s cloud‑based storage and synchronization service that backs up device data, settings, photos, and app information to the cloud. It enables users to restore their devices from a recent snapshot and keep files accessible across Apple devices.

## Role in [[summaries/session-02_2024-06-15]]
In the beta‑testing checklist, iCloud is recommended as the primary cloud backup for phones before installing beta updates. The conversation stresses creating a fresh iCloud backup, then supplementing it with a manual local backup to ensure a reliable restore point.

## Key Practices Mentioned
- **Fresh backup**: Update the iCloud backup immediately before a beta install.
- **Verification**: Check the backup timestamp and confirm the backup file exists before proceeding.
- **Rollback**: Use the iCloud snapshot together with a local backup to restore the phone in under an hour if the beta fails.

## Related Concepts
- [[concepts/software-update-strategy]] – balancing timely updates with stability.
- [[concepts/beta-testing-risk-management]] – mitigation tactics for beta installs.
- [[concepts/device-isolation]] – using secondary devices to protect primary workflows.

## Related Entities
- [[entities/google-drive]] – another cloud backup option mentioned as an alternative.
- [[entities/time-machine]] – macOS backup solution comparable to iCloud for laptops.
- [[entities/file-history]] – Windows backup tool referenced alongside iCloud.
- [[entities/microsoft]] – broader ecosystem within which file‑history operates.

## See Also
- [[index]]
