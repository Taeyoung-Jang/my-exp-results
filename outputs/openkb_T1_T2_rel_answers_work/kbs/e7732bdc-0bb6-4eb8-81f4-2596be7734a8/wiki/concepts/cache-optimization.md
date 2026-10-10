---
type: "Concept"
sources: ["summaries/session-31_2025-03-14.md"]
description: "Guidelines for organizing and tuning media caches to maximize performance in video/3D workflows."
---

# Cache Optimization

Cache optimization is the practice of configuring media cache locations, formats, and sizes to keep video‑editing and 3D‑rendering applications running smoothly, especially under sustained heavy loads.

## Why it matters
- **Bandwidth contention**: When the operating system, project files, raw footage, and cache all share a single drive, read/write throughput can become a bottleneck.
- **Playback stutter**: Insufficient or poorly placed cache forces applications to repeatedly fetch data from slower storage, causing frame drops.
- **Render delays**: Rendering engines that rely on temporary files (e.g., proxy renders, intermediate frames) suffer if the cache is on a congested drive.

## Key strategies (derived from [[summaries/session-31_2025-03-14]])
1. **Dedicated cache drive**
   - Use a separate fast NVMe drive for cache and scratch files. This isolates high‑frequency I/O from the OS and media drives.
   - Align with [[concepts/nvme-storage]] for low latency and high sequential throughput.
2. **Drive layout**
   - **Drive 1**: OS and applications.
   - **Drive 2**: Project files and raw footage.
   - **Drive 3**: Cache/scratch (Resolve cache, After Effects disk cache, optimized media).
   - A three‑drive setup is noticeably better than a two‑drive configuration when working with 8K or heavy compositing.
3. **Cache format selection**
   - Choose efficient, intra‑frame codecs for cache files. The source recommends ProRes or DNxHR, which balance quality and decode speed.
   - These are represented by the entities [[entities/prores]] and [[entities/dnxhr]].
4. **Size allocation**
   - Increase the disk‑cache size in After Effects to a level where old frames rarely need to be evicted.
   - In DaVinci Resolve, set the cache format to the chosen codec and allocate ample space on the dedicated cache drive.
5. **Thermal and power considerations**
   - Keep the GPU and CPU temperatures low to avoid throttling, which indirectly affects cache performance by maintaining consistent I/O rates.

## Practical checklist
- [ ] Verify each drive is an NVMe SSD (or equivalent high‑speed storage).
- [ ] Configure DaVinci Resolve cache location to the dedicated cache drive and set the format to [[entities/prores]] or [[entities/dnxhr]].
- [ ] Set After Effects "Disk Cache" path to the same dedicated drive and raise the cache size.
- [ ] Monitor drive utilization during a heavy session; aim for < 80 % sustained bandwidth usage.
- [ ] Periodically clean old cache files to free space and prevent fragmentation.

## Related concepts
- [[concepts/gpu-vram]] – sufficient VRAM reduces reliance on cache for large textures.
- [[concepts/nvme-storage]] – the hardware foundation for effective cache.
- [[concepts/export-settings]] – export pipelines often reuse cache files; aligning export formats with cache formats can speed up final renders.

---
*This concept page synthesizes recommendations from [[summaries/session-31_2025-03-14]] and provides a reusable framework for optimizing cache workflows in professional video and 3D production environments.*