---
sources: ["summaries/session-31_2025-03-14.md"]
type: "Product"
description: "Blender is an open‑source 3D creation suite for modeling, rendering, and animation."
---

# Blender (product)

## Overview
Blender is a free, open‑source 3D creation suite used for modeling, sculpting, animation, simulation, rendering, compositing, and motion‑tracking. It includes the **Cycles** render engine, which can leverage GPU acceleration for fast renders.

## Mention in [[summaries/session-31_2025-03-14]]
In the *session‑31* discussion, Blender (Cycles) was cited alongside DaVinci Resolve and After Effects as a primary workload. The advice focused on:
- Prioritising a GPU with ample [[concepts/gpu-vram]] (≥ 16 GB) because Cycles scales directly with GPU memory and compute power.
- Ensuring fast NVMe storage ([[concepts/nvme-storage]]) for project files, raw footage, and cache to avoid bottlenecks.
- Using proper cache settings (see [[concepts/cache-optimization]]) to keep playback smooth during heavy 8K sessions.

## Hardware recommendations for optimal Blender performance
- **GPU**: High‑end NVIDIA or AMD cards with ≥ 16 GB VRAM; larger VRAM helps prevent texture swaps during complex 8K renders.
- **CPU**: While Blender’s GPU path is primary, a CPU with strong single‑core performance (8‑12 cores) benefits UI responsiveness and any CPU‑only passes.
- **RAM**: 64 GB is the minimum for comfortable 8K workflows; 128 GB removes most memory‑to‑disk spills.
- **Storage**: A dedicated NVMe drive for cache/scratch, separate from OS and media drives, maximises throughput.

## Interaction with other tools
Blender often shares the same workstation as [[entities/davinci-resolve]] and [[entities/after-effects]], so the hardware choices that benefit Blender also benefit those applications. The recommendation to use NVIDIA GPUs aligns with the broader ecosystem’s reliance on CUDA for accelerated rendering.

---
*This entity page aggregates the key facts about Blender from the session‑31 discussion.*