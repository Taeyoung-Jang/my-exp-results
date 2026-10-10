---
sources: ["summaries/session-15_2023-06-15.md"]
type: "Product"
description: "ProRes Proxy is a lightweight intermediate codec used for proxy editing on low-end systems."
---

## ProRes Proxy

ProRes Proxy is an intermediate video codec designed for fast decoding and modest file sizes. It is often packaged in a **.mov** container and is popular for proxy workflows on modest hardware because it balances quality and CPU load.

### Key facts from [[summaries/session-15_2023-06-15]]
- Recommended as a proxy format for **Shotcut** and **Kdenlive** when editing 1080p 60 fps phone footage on an older Windows 10 PC (quad‑core CPU, 8 GB RAM, 2 GB GPU).
- Suggested resolution: **720p** proxies to keep playback smooth while preserving enough detail for editing.
- Compared with [[entities/dnxhr-lb]] (DNxHR LB) – both are viable, but DNxHR LB in an MXF container may decode slightly faster on Windows; ProRes Proxy offers broader cross‑platform compatibility.
- Used as part of the overall [[concepts/proxy-workflow]] to off‑load the main CPU during editing, allowing the timeline to run at full resolution only for final renders.

### Relationship to concepts
- Supports the [[concepts/low-end-video-editing]] approach by providing a codec that can be decoded with minimal GPU strain.
- Integral to a robust [[concepts/proxy-workflow]] for low‑spec machines.
- Fits within [[concepts/windows-performance-tweaks]] by enabling the user to store proxies on an SSD and reduce RAM pressure.

### Practical tips (derived from the session)
1. **Create proxies**: In Kdenlive, enable *Use Proxies* under *Project Settings → Proxies* and select the *ProRes Proxy 720p* profile.
2. **Storage**: Point the proxy folder to a fast SSD via *Settings → Configure Kdenlive → Project Defaults → Proxy*.
3. **Shotcut limitation**: Modern builds of Shotcut only toggle proxy generation on/off and lack direct codec selection; if precise control is needed, Kdenlive is recommended.
4. **Verification**: After conversion, use [[entities/mediainfo]] to confirm the proxy file properties (codec = ProRes, resolution = 720p, constant frame rate).

### Alternative
- For users who prefer an MXF container, [[entities/dnxhr-lb]] is a solid alternative, especially on Windows where it may decode more efficiently.

---
*Entity page for **ProRes Proxy**, a product referenced in the session‑15 discussion of low‑end video editing workflows.*