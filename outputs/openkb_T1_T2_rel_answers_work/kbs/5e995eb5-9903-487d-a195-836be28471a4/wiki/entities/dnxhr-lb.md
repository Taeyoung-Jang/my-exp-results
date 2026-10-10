---
sources: ["summaries/session-15_2023-06-15.md"]
type: "Product"
description: "DNxHR LB is a low‑bitrate intra‑frame codec often used for editing proxies."
---

# DNxHR LB (product)

DNxHR LB (Low‑Bandwidth) is an intra‑frame video codec designed for efficient editing workflows. It stores each frame as an independent image, which makes it quick to decode on modest hardware. In the context of [[summaries/session-15_2023-06-15]], DNxHR LB is recommended as the preferred proxy codec for low‑end Windows machines when using [[entities/kdenlive]].

## Why use DNxHR LB for proxy‑workflow?
- **Performance**: The codec’s intra‑frame nature and relatively low bitrate allow smooth playback on older CPUs and GPUs with limited RAM.
- **Container**: It is typically wrapped in an MXF container, which Windows handles efficiently.
- **Comparison**: While [[entities/prores-proxy]] (MOV) offers cross‑platform compatibility, DNxHR LB tends to decode slightly faster on Windows, making it the safer choice for [[concepts/low-end-video-editing]].

## How it fits into the recommended workflow
1. **Proxy creation**: In Kdenlive’s Project Settings → Proxies tab, the user selects the *DNxHR LB 720p* profile. This creates 720 p proxy files that keep the original frame‑rate (e.g., 59.94 fps) while dramatically reducing CPU load.
2. **Storage**: Proxies are stored on an SSD to benefit from faster read/write speeds, aligning with [[concepts/windows-performance-tweaks]].
3. **Editing**: The lightweight proxies allow real‑time editing without stutter, and the final render can switch back to the full‑resolution source.

## Related tools and entities
- **[[entities/kdenlive]]** – the video editor where DNxHR LB proxies are configured.
- **[[entities/shotcut]]** – mentioned as an alternative editor, though its current proxy UI does not expose codec selection.
- **[[entities/handbrake]]** – used to convert variable‑frame‑rate footage to a constant frame rate before proxy generation.
- **[[entities/mediainfo]]** – employed to verify that exported footage has a consistent frame rate.

## Summary
DNxHR LB provides a balance of decoding speed and manageable file size, making it ideal for the proxy‑workflow recommended for low‑spec Windows PCs. Its use in the session‑15 guidance helps achieve smooth playback and efficient editing when combined with appropriate system tweaks and SSD‑based cache locations.