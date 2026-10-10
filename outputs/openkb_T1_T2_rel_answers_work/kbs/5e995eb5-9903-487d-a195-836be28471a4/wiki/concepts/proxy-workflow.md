---
type: "Concept"
sources: ["summaries/session-37_2024-06-15.md", "summaries/session-15_2023-06-15.md"]
description: "A method of using low‑resolution proxy files to enable smooth editing on limited hardware."
---

# Proxy Workflow

**Definition** – A proxy workflow consists of generating lower‑resolution, lightweight versions of source media (proxies) and using those proxies for editing, while keeping the original high‑quality files for final rendering. This approach is essential for [[concepts/low-end-video-editing]] because it reduces CPU, GPU, and RAM load during playback and trimming.

## Core Steps (as applied in [[summaries/session-15_2023-06-15]])
1. **Create proxies** – Convert each source clip to a 720p (or 540p when necessary) proxy using a codec that decodes efficiently on modest hardware. Common choices are **DNxHR LB** in an MXF container ([[entities/dnxhr-lb]]) or **ProRes Proxy** in MOV ([[entities/prores-proxy]]).
2. **Match frame rate** – Maintain the original frame rate (e.g., 59.94 fps or 60 fps) when generating proxies to avoid audio drift. For variable‑frame‑rate phone footage, first convert to constant frame rate with **HandBrake** ([[entities/handbrake]]) and verify with **MediaInfo** ([[entities/mediainfo]]).
3. **Configure the editor** – Enable proxy usage in the editing application and point the proxy folder to a fast SSD. In **Kdenlive** ([[entities/kdenlive]]) this is done via *Project → Project Settings → Proxies* and *Settings → Configure Kdenlive → Project Defaults → Proxy*. In **Shotcut** ([[entities/shotcut]]) the proxy toggle is under *Settings → Proxy* (codec selection is limited, so Kdenlive is often preferred for precise control).
4. **Edit using proxies** – Work on the low‑resolution files; set the preview scaling to half or quarter resolution to further lighten the load.
5. **Final render** – Switch back to the original high‑resolution media for export. Use an H.264 preset at 12‑16 Mbps for 1080p output, selecting a medium encode speed to balance quality and render time.

## Benefits
- **Performance** – Reduces decoding workload, preventing stutters on CPUs with few cores and limited RAM.
- **Flexibility** – Allows editors to keep the original footage untouched while still experimenting with cuts and effects.
- **Resource Management** – By storing proxies and cache on an SSD, the workflow aligns with [[concepts/windows-performance-tweaks]] such as moving temporary data off slower drives.

## Related Concepts
- [[concepts/low-end-video-editing]] – broader strategies for editing on constrained hardware.
- [[concepts/windows-performance-tweaks]] – system‑level adjustments that complement a proxy workflow.


See also: [[summaries/session-37_2024-06-15]]