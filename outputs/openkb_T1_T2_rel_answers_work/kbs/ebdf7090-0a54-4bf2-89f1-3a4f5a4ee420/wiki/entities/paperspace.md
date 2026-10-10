---
sources: ["summaries/session-01_2025-06-15.md"]
type: "Product"
description: "Cloud‑based GPU workstation service for high‑performance rendering."
---

# Paperspace

Paperspace is a cloud computing platform that provides virtual machines equipped with powerful GPUs, enabling users to run demanding applications like video editing and rendering without relying on local hardware.

## Relevance to session‑01_2025‑06‑15
- Suggested as a **cloud/offload option** for exporting large‑scale Premiere Pro projects when the local machine cannot handle an 8K render.
- Allows editors to **rent a GPU‑enabled VM**, install [[entities/adobe-premiere-pro]], and perform the final master export using the same **[[concepts/mezzanine-codec]]** settings (e.g., DNxHR HQ).
- Works well with the **[[concepts/chunked-export]]** workflow: export 5‑10 minute chunks locally or on a modest workstation, then stitch and render the final master on Paperspace to avoid crashes.

## Key Features
- **GPU‑accelerated virtual desktops** (NVIDIA RTX series) suitable for 8K video processing.
- **Flexible billing** (hourly or monthly) letting users scale resources to match render demands.
- Supports **Windows** environments, which is required for the DNxHR workflow discussed in the session.
- Easy integration with **Adobe Team Projects** for collaborative editing and remote rendering.

## Related Entities and Concepts
- [[entities/aws-ec2-g-series]] – another cloud GPU option mentioned alongside Paperspace.
- [[entities/adobe-team-projects]] – collaborative platform that can be used in conjunction with Paperspace for remote rendering.
- [[entities/adobe-premiere-pro]] – the editing software for which Paperspace can provide the needed compute power.
- [[concepts/proxy-workflow]] – can be employed before offloading the final render to Paperspace.
- [[summaries/session-01_2025-06-15]] – the source conversation that references Paperspace as a recommended solution.