---
sources: ["summaries/session-05_2024-06-15.md"]
type: "Product"
description: "Compact, low‑power mini PC often used as a home media server."
---

# Intel NUC

Intel NUC (Next Unit of Computing) is a small, low‑power desktop computer often used as a home media server. In the context of [[summaries/session-05_2024-06-15]], it was recommended as the hardware platform for ripping Blu‑rays and CDs and streaming the resulting library to TVs and mobile devices.

## Why it’s suggested
- Compact size fits easily into a home entertainment setup.
- Sufficient processing power to run media‑server software such as [[entities/plex]] or [[entities/jellyfin]] and handle transcoding tasks.
- Can host ripping tools like [[entities/makemkv]] and [[entities/handbrake]] for converting discs to digital files.

## Role in balancing convenience and ownership
The Intel NUC enables the workflow described in [[concepts/convenience_vs_ownership]], allowing users to keep physical media while gaining digital convenience. By pairing the NUC with a disc drive, users can perform [[concepts/disc_ripping]] and store DRM‑free copies, aligning with the principles of [[concepts/drm_free_downloads]].

## Typical setup
1. Connect an external Blu‑ray drive.
2. Use MakeMKV to rip Blu‑rays, then HandBrake to encode them.
3. Serve the library via Plex or Jellyfin running on the NUC.
4. Access the media on TVs, phones, or tablets over the home network.

## Related entities
- [[entities/handbrake]]
- [[entities/jellyfin]]
- [[entities/makemkv]]
- [[entities/plex]]