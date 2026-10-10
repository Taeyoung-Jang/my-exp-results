---
sources: ["summaries/session-15_2023-06-15.md"]
type: "Product"
description: "Kdenlive is a lightweight, open‑source video editor suited for low‑end hardware."
---

# Kdenlive

Kdenlive is an open‑source, cross‑platform video editing application that is well‑suited for **low‑end video editing** scenarios. In the context of the *session‑15_2023‑06‑15* discussion, it is recommended as a primary editor (with Shotcut as an alternative) for a Windows 10 machine with a quad‑core CPU, 8 GB RAM, and a modest 2 GB GPU.

## Key Features Highlighted
- **Proxy workflow**: Kdenlive’s built‑in proxy system allows users to generate low‑resolution, low‑bitrate proxy files (e.g., DNxHR LB 720p) to enable smooth playback while editing high‑resolution source footage.
- **Configurable proxy and cache locations**: Users can set the proxy folder and the preview/render cache folder to an SSD via the *Configure Kdenlive* dialog, improving performance on limited RAM.
- **Project settings**: The editor supports matching the project frame rate to source footage (typically 59.94 fps for phone video) to avoid audio drift and stutter.
- **Export presets**: Recommended export uses H.264 at 12‑16 Mbps with a medium encode speed, balancing quality and render time on older CPUs.

## Recommended Settings from the Session
1. **Enable proxies** – *Project → Project Settings → Proxies* tab, turn on *Use Proxies*.
2. **Select proxy profile** – Choose the *DNxHR LB 720p* profile (or *ProRes Proxy 720p* for cross‑platform compatibility).
3. **Set proxy folder** – *Settings → Configure Kdenlive → Project Defaults → Proxy* → point to an SSD.
4. **Set cache folder** – *Settings → Configure Kdenlive → Miscellaneous* → set *Cache data folder* to the same SSD.
5. **Timeline** – Keep project resolution at 1080p, preview scaling at half or quarter quality.

## Related Tools & Concepts
- The proxy workflow ties closely to [[concepts/proxy-workflow]] and the need for [[concepts/low-end-video-editing]].
- Performance improvements on Windows 10, such as moving caches to an SSD and disabling background apps, relate to [[concepts/windows-performance-tweaks]].
- For converting variable‑frame‑rate footage before import, the workflow suggests using [[entities/handbrake]] and verifying results with [[entities/mediainfo]].
- While Kdenlive is the focus, the discussion also references [[entities/shotcut]] as an alternative editor and [[entities/blender]] for lightweight 3‑D work.

## Reference
This information is drawn from the summary of the conversation documented in [[summaries/session-15_2023-06-15]].