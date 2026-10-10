---
sources: ["summaries/session-40_2025-10-15.md"]
type: "Product"
description: "A portable USB drive used to move results from an offline workstation to the main computer."
---

# USB Transfer

**Type:** Product  
**Description:** A portable USB drive used to move results from an offline workstation to the main computer.

## Role in Session 40 (2025‑10‑15)

In [[summaries/session-40_2025-10-15]], the USB Transfer is the sole physical medium for the daily hand‑off of data. The workflow prescribes:

- Plugging the drive once each morning after the offline run finishes.
- Copying the entire `bundle/` folder (logs, outputs, status) in a single operation.
- Unplugging immediately to avoid “distraction loops” and keep the offline environment sealed.

## Relationship to Concepts

The device supports the [[concepts/offline_compute_workflow]] by providing a reliable, isolated channel for moving artifacts while maintaining a distraction‑free environment. It also contributes to a focused [[concepts/deep_work_environment]] by limiting the need for frequent computer‑to‑computer interaction.

## Interaction with Other Entities

The hand‑off process is coordinated with the run‑locking mechanism [[entities/run_lock]] to ensure that the offline job is not active while the drive is being accessed.

## Practical Tips

- Use a dedicated USB stick for this purpose only; label it clearly.
- Keep the drive empty before each night’s run so the transfer bundle is the only content.
- Verify the copy with a simple checksum (e.g., `sha256sum`) before unplugging.