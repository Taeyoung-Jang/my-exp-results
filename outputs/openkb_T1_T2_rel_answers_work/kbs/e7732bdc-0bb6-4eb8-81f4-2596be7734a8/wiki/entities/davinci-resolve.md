---
sources: ["summaries/session-31_2025-03-14.md"]
type: "Product"
description: "Professional video editing and colour‑grading software for high‑resolution workflows"
---

# DaVinci Resolve

DaVinci Resolve is a professional video editing, colour‑grading, visual‑effects, and audio‑post‑production suite.

## Key points from [[summaries/session-31_2025-03-14]]
- **GPU focus**: Performance is tightly coupled to GPU power and especially to VRAM capacity. The session recommends a minimum of **16 GB VRAM** (24 GB preferred) for smooth 8K timelines.
- **CPU role**: Although Resolve leans on the GPU, a fast CPU with strong single‑core performance (8‑12 cores) is advised for encoding and non‑GPU tasks.
- **Memory**: At least **64 GB RAM** is suggested as the floor for 8K editing; 128 GB eliminates most paging concerns.
- **Storage layout**: A dedicated fast **NVMe** drive for cache and scratch material yields the best responsiveness. The session highlights the benefit of a three‑drive configuration (OS/apps, media, cache) and links this to the concept of [[concepts/nvme-storage]].
- **Cache optimisation**: Resolve works best when its cache is placed on an isolated fast drive and when cache formats such as **ProRes** or **DNxHR** are used. See also [[concepts/cache-optimization]].
- **Workflow extras**: The discussion mentions that workstation features like ECC RAM, Thunderbolt, and 10 GbE are optional for most creative users.

## Related entities and concepts
- [[entities/blender]] – often paired with Resolve for 3D assets.
- [[entities/after-effects]] – another key application in the same workflow.
- [[concepts/gpu-vram]] – the critical GPU memory factor.
- [[concepts/nvme-storage]] – fast storage recommendation.
- [[concepts/cache-optimization]] – improving Resolve’s cache performance.

---