---
type: "Concept"
sources: ["summaries/session-31_2025-03-14.md"]
description: "GPU VRAM is the video memory on graphics cards that determines performance for high‑resolution video and 3D workloads."
---

# GPU VRAM

**Definition**: GPU VRAM (Video Random Access Memory) is the dedicated memory on a graphics card used to store textures, frame buffers, and compute data for rendering tasks. It is a critical resource for video editing, color grading, and 3D rendering because it determines how much high‑resolution media and how many complex scene assets can be held in fast, on‑card storage during processing.

---

## Why VRAM matters for creative workflows
- **8K and high‑resolution timelines**: Large frame buffers and raw footage quickly consume memory. The session‑31 discussion recommends a **minimum of 16 GB VRAM** for comfortable 8K editing in DaVinci Resolve, with **24 GB** providing a more future‑proof headroom.
- **Complex 3D scenes**: In Blender's Cycles engine, each texture, geometry cache, and lighting calculation resides in VRAM. Insufficient VRAM forces the renderer to fall back to system RAM or disk, causing severe slow‑downs.
- **After Effects compositing**: High‑resolution layers and effects are cached in VRAM; running out can trigger frame‑rate drops and increased GPU paging.
- **Cache and scratch performance**: Even when using fast [[concepts/nvme-storage]], a bottleneck can appear if the GPU must swap data between VRAM and system memory.

---

## Recommended VRAM sizing (based on the source session)
| Use‑case | Minimum VRAM | Recommended VRAM |
|----------|--------------|------------------|
| 8K video editing (Resolve) | 16 GB | 24 GB |
| Heavy 3D rendering (Blender Cycles) | 16 GB | 24 GB |
| General 4K/6K work | 12 GB | 16 GB |

---

## Trade‑offs and selection tips
1. **Prioritize VRAM over raw clock speed** when your primary tasks are GPU‑accelerated video editing or path‑traced rendering.
2. **Balance with system RAM**: 64 GB–128 GB RAM is advised so the GPU can offload overflow without resorting to disk swapping.
3. **Future‑proofing**: Choose a card with the highest VRAM you can afford; software updates often increase memory demands.

---

## Related concepts and entities
- [[concepts/cache-optimization]] – how cache placement interacts with VRAM limits.
- [[concepts/nvme-storage]] – fast storage mitigates but does not replace VRAM capacity.
- [[entities/davinci-resolve]] – heavily VRAM‑dependent for 8K timelines.
- [[entities/blender]] – utilizes VRAM for Cycles rendering.
- [[entities/after-effects]] – relies on VRAM for high‑resolution compositing.

---

## Source reference
This concept is drawn from the discussion in [[summaries/session-31_2025-03-14]], which emphasized VRAM as the top hardware priority for 8K video and 3D workloads.
