---
sources: ["summaries/session-15_2023-06-15.md"]
type: "Product"
description: "HandBrake is an open‑source video transcoder used to convert media files."
---

# HandBrake (product)

**Overview**
HandBrake is a free, open‑source video transcoding application that supports a wide range of input formats and provides extensive options for output encoding, frame‑rate control, and container selection.

**Key facts from [[summaries/session-15_2023-06-15]]**
- Recommended as the tool to convert variable‑frame‑rate phone footage to a constant frame rate before editing.
- Suggested preset: *Fast 1080p30* (adjusted for 1080p 60 fps sources).
- In the **Video** tab, set the frame‑rate dropdown to **59.94** or **60**, enable **Constant Framerate**, and use H.264 with an RF of 18‑20 (≈20‑25 Mbps).
- HandBrake is part of the recommended [[concepts/proxy-workflow]] for a smooth low‑end video editing pipeline.

**Why it matters for [[concepts/low-end-video-editing]]**
Converting source clips to a constant frame rate and a manageable codec reduces CPU load during proxy generation and playback, which is crucial on older hardware with limited RAM and GPU resources.

**Integration with the workflow**
1. Open the source clip in HandBrake.
2. Choose the *Fast 1080p30* preset as a base.
3. Switch the *Framerate* dropdown to the desired constant rate (59.94 fps is a safe default for most phones).
4. Tick **Constant Framerate**.
5. Set the video codec to H.264, RF 18‑20, or an average bitrate of 20‑25 Mbps.
6. Start the conversion and verify the output with [[entities/mediainfo]].

**Verification**
After encoding, load the exported file in MediaInfo. A proper constant‑frame‑rate file shows a single fixed “Frame rate” value (e.g., 59.940 fps) with no mention of “Variable” or min/max rates.

**Related entities**
- [[entities/kdenlive]] – the editor that can ingest the HandBrake‑converted files.
- [[entities/shotcut]] – an alternate editor; also benefits from HandBrake‑produced CFR clips.
- [[entities/dnxhr-lb]] and [[entities/prores-proxy]] – proxy codecs mentioned alongside HandBrake in the workflow.
- [[entities/blender]] – 3‑D software that may use the same source footage after HandBrake conversion.

**Performance considerations**
Using HandBrake to standardize frame rate aligns with the [[concepts/windows-performance-tweaks]] advice of minimizing background processing and keeping the editing pipeline lightweight.
