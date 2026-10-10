---
type: "Concept"
sources: ["summaries/session-37_2024-06-15.md", "summaries/session-15_2023-06-15.md"]
description: "Strategies and tools for editing video efficiently on limited‑hardware systems."
---

# Low‑End Video Editing

**Definition** – A workflow that enables smooth editing of high‑resolution footage on computers with modest CPU, RAM, and GPU resources.

## Core Principles
- **Lightweight editors** – Choose software with low resource demands. The session recommends **Shotcut** as the primary choice and **Kdenlive** as a reliable backup.
- **Proxy workflow** – Convert source clips to lower‑resolution, low‑bitrate proxies before editing. This dramatically reduces decode load while preserving timing.
- **Resolution & frame‑rate matching** – Keep the project timeline at the original resolution (e.g., 1080p) but set preview scaling to half or quarter quality. Match the timeline FPS to the source (typically 59.94 fps for phone footage) to avoid stutter and audio drift.
- **Export settings** – Use H.264 at a moderate bitrate (12‑16 Mbps for 1080p) and a "medium" encode speed. Avoid max‑quality presets that heavily tax the CPU.
- **System tweaks** – Store project files, proxies, and cache on the fastest drive (SSD), close background applications, and turn off Windows visual effects.

## Recommended Tools & Settings (from [[summaries/session-15_2023-06-15]])
| Task | Recommended Tool | Settings / Tips |
|------|------------------|-----------------|
| Editing UI | **Shotcut** (primary) or **Kdenlive** (fallback) | Enable proxies; use Shotcut’s simple on/off proxy toggle or Kdenlive’s detailed proxy profile selection. |
| Proxy codec | **DNxHR LB** (MXF) or **ProRes Proxy** (MOV) | DNxHR LB often decodes faster on Windows; ProRes Proxy offers cross‑platform compatibility. |
| Proxy resolution | 720p (default) – drop to 540p if still sluggish |
| Frame‑rate handling | Convert variable‑frame‑rate footage to constant using **HandBrake** (see [[entities/handbrake]]) | Set to 59.94 fps or 60 fps; enable *Constant Framerate*.
| 3‑D elements | Use **Blender** with Eevee for real‑time previews; keep Cycles samples low |
| System performance | Apply [[concepts/windows-performance-tweaks]] such as SSD cache placement and disabling visual effects |

## Workflow Overview
1. **Convert VFR source** – Run phone clips through HandBrake, selecting a constant frame rate (59.94 fps) and H.264 quality around 20‑25 Mbps.
2. **Generate proxies** – In Kdenlive, turn on *Use Proxies* and select the DNxHR LB 720p profile; in Shotcut, enable the proxy toggle and let it create default low‑res proxies.
3. **Edit** – Work on the low‑res proxies, keep preview scaling low, and avoid heavy filters until the final render.
4. **Render 3‑D assets** – If needed, render Blender output at modest resolution and denoise.
5. **Final export** – Switch back to full‑res media, export with H.264 at 12‑16 Mbps, medium speed.

## Related Concepts
- [[concepts/proxy-workflow]] – the detailed proxy creation and usage process.
- [[concepts/windows-performance-tweaks]] – OS‑level adjustments for low‑memory systems.
- [[concepts/low-end-video-editing]] – this page itself serves as the hub for the overarching strategy.

*This concept is derived from the advice given in [[summaries/session-15_2023-06-15]].*

See also: [[summaries/session-37_2024-06-15]]