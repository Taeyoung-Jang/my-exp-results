---
sources: ["summaries/session-15_2023-06-15.md"]
type: "Product"
description: "Lightweight video editor for Windows, suited to low‑end hardware with basic proxy support."
---

# Shotcut

Shotcut is an open‑source, cross‑platform video editor that runs well on older Windows 10 machines. In the context of [[summaries/session-15_2023-06-15]], it was recommended as the primary editing tool for a system with a quad‑core CPU, 8 GB RAM, and a modest 2 GB GPU because of its minimal resource footprint.

## Key Facts from the Session Document
- **Proxy workflow** – Shotcut offers an on/off proxy toggle under the **Settings → Proxy** menu. While it does not expose codec or resolution choices directly, enabling proxies moves low‑resolution versions of source clips to a user‑specified storage location, improving playback smoothness for [[concepts/low-end-video-editing]].
- **Proxy format limitation** – The UI does not let users pick between [[entities/prores-proxy]] or [[entities/dnxhr-lb]]; it simply creates intermediate files using its internal default. For users needing specific codec control, the document suggests switching to [[entities/kdenlive]], which provides explicit proxy profiles.
- **Performance tweaks** – To maximize responsiveness, the user should point Shotcut’s cache and proxy folders to an SSD and close background applications, aligning with [[concepts/windows-performance-tweaks]].
- **Workflow integration** – The recommended workflow pairs Shotcut with **HandBrake** for converting variable‑frame‑rate phone footage to constant frame rate before import, and with **MediaInfo** for verifying the conversion.

## Typical Usage Scenario
1. Open **Settings → Proxy** and enable *Use Proxy*.
2. Set the *Proxy storage* folder to a fast SSD.
3. Import 1080p 60 fps footage (after optional CFR conversion with [[entities/handbrake]]).
4. Edit at full resolution while Shotcut automatically serves low‑resolution proxies for smoother playback.
5. Export the final project using H.264 at 12‑16 Mbps, avoiding high‑quality presets to keep render times short.

## Related Concepts and Entities
- [[concepts/proxy-workflow]] – The overall strategy of using lower‑resolution stand‑ins during editing.
- [[concepts/low-end-video-editing]] – Strategies and tools for editing on limited hardware.
- [[concepts/windows-performance-tweaks]] – System adjustments that complement Shotcut’s lightweight nature.
- [[entities/kdenlive]] – An alternative editor with richer proxy configuration options.
- [[entities/blender]] – Mentioned for basic 3D work that can be integrated into Shotcut timelines.

## References
The recommendations above are drawn from the conversation in [[summaries/session-15_2023-06-15]], which details the step‑by‑step proxy setup, VFR conversion, and Windows performance tips specific to the user's hardware.