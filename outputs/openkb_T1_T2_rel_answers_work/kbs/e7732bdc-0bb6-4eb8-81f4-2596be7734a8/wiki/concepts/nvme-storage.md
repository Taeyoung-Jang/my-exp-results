---
type: "Concept"
sources: ["summaries/session-31_2025-03-14.md"]
description: "High‑speed SSD storage used for OS, media, and cache in creative workflows"
---

# NVMe Storage

## Definition
NVMe (Non‑Volatile Memory Express) storage refers to solid‑state drives that connect directly to the PCIe bus, delivering significantly higher throughput and lower latency than SATA SSDs. In creative workstations the fast read/write speeds are crucial for handling large media files, project caches, and scratch disks without becoming a bottleneck.

## Why it matters for video/3D editing
In the discussion of [[summaries/session-31_2025-03-14]] the assistant highlights that storage contention is one of the most overlooked performance limits. Resolve, Blender Cycles, and After Effects constantly read raw footage, write intermediate renders, and access cache files. A single NVMe drive can become saturated when these tasks share bandwidth, leading to stutters and longer render times.

## Recommended drive layout
| Setup | Purpose | Benefit |
|-------|---------|---------|
| **2‑drive NVMe** | Drive 1: OS & apps; Drive 2: media, project files, cache | Works for many workflows but the OS and cache share bandwidth during heavy renders.
| **3‑drive NVMe** | Drive 1: OS & apps; Drive 2: raw footage & project files; Drive 3: Resolve cache, After Effects disk cache, optimized media | Isolates high‑traffic cache I/O, reducing contention and keeping playback smooth, especially in 8K timelines.

The summary notes that while a two‑drive configuration is “workable,” a third dedicated cache/scratch drive becomes “noticeably better” for sustained 6K–8K workloads.

## Interaction with other concepts
- Sufficient **[[concepts/gpu-vram]]** (≥ 16 GB) prevents the GPU from falling back to system memory, but the storage layer still needs to feed the GPU fast enough.
- Proper **[[concepts/cache-optimization]]** (e.g., using ProRes or DNxHR proxies) amplifies the benefits of a fast NVMe layout, as cache files are written and read at high speed.

## Best‑practice checklist
1. Use at least one NVMe drive for the operating system and applications.
2. Allocate a second NVMe drive for raw media and project files.
3. Add a third NVMe drive dedicated to cache/scratch if your workflow regularly handles 8K or multi‑layer compositions.
4. Pair the storage plan with a GPU that has ample VRAM and sufficient RAM (64 GB+), as outlined in the same session.
5. Regularly monitor drive health and maintain free space to avoid performance degradation.

## Source
The recommendations are drawn directly from the conversation in [[summaries/session-31_2025-03-14]].