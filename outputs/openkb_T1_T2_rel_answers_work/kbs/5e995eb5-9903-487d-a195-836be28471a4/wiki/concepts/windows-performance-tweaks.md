---
type: "Concept"
sources: ["summaries/session-15_2023-06-15.md"]
description: "Tips to optimise Windows 10 for video editing on limited‑resource PCs."
---

# Windows Performance Tweaks

**Scope** – Practical adjustments for Windows 10 systems with modest hardware (e.g., quad‑core CPU, 8 GB RAM, low‑end GPU) to keep video‑editing workflows smooth.

## Core Strategies

1. **Place heavy data on the fastest drive**
   - Store project files, proxy media, and cache directories on an SSD. This reduces I/O latency and prevents the HDD from becoming a bottleneck during playback and rendering.
2. **Limit background RAM usage**
   - Close browsers, chat clients, launchers, and any non‑essential software before launching the editor. Even lightweight apps can consume a few hundred megabytes, which matters when the system only has 8 GB.
3. **Disable Windows visual effects**
   - Open *Settings → Personalization → Colors* and turn off transparency effects. Optionally, in *System → Advanced system settings → Performance* select “Adjust for best performance” to turn off animations, shadows, and other GPU‑intensive UI features.
4. **Configure editor cache locations**
   - In [[entities/kdenlive]] go to **Settings → Configure Kdenlive → Miscellaneous** and set the *Cache data folder* to the SSD.
   - In [[entities/shotcut]] enable proxies (Settings → Proxy) and point the *Proxy Storage* folder to the SSD as well.
5. **Optimize power settings**
   - Choose the “High performance” plan in *Control Panel → Power Options* to prevent the CPU from throttling during intensive encode tasks.
6. **Keep the system updated**
   - Install the latest Windows updates and driver versions for the GPU and storage controller to benefit from performance improvements and bug fixes.

## Interaction with Other Concepts

- These tweaks complement a robust **[[concepts/proxy-workflow]]** by ensuring that proxy generation and playback are not slowed by disk bottlenecks.
- When combined with a **[[concepts/low-end-video-editing]]** approach (lightweight editors, reduced preview resolution), the overall editing experience becomes fluid even on older hardware.

## Reference

The recommendations are drawn from the practical guide provided in [[summaries/session-15_2023-06-15]], which detailed a step‑by‑step workflow for Shotcut and Kdenlive on a low‑spec Windows 10 machine.