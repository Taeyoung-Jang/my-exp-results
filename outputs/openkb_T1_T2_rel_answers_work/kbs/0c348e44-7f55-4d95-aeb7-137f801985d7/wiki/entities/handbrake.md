---
sources: ["summaries/session-05_2024-06-15.md"]
type: "Product"
description: "HandBrake is an open‑source video transcoder for converting ripped media."
---

# HandBrake

**Type:** Product

HandBrake is a free, open‑source video transcoding tool that converts video files from one format to another. It is widely used to re‑encode ripped Blu‑ray or DVD content into more manageable sizes and formats for playback on various devices.

---

## Role in [[summaries/session-05_2024-06-15]]

In the "session-05_2024-06-15" conversation, HandBrake is recommended as the encoder to process Blu‑ray rip files after extracting them with [[entities/makemkv]]. The workflow suggested:
1. Rip the disc with MakeMKV.
2. Use HandBrake to encode the raw video into a space‑efficient, device‑compatible format.
3. Serve the encoded files via a media server such as [[entities/plex]] or [[entities/jellyfin]].

---

## Key Features Highlighted
- **Format flexibility:** Supports a wide range of output containers (MP4, MKV, etc.).
- **Presets:** Provides device‑specific presets that simplify creating files suitable for TVs, phones, and tablets.
- **Open source:** No licensing fees, aligning with the goal of maintaining true ownership of media.

---

## Related Tools and Concepts
- **[[entities/makemkv]]** – Used to extract the original video and audio streams from Blu‑ray discs before handing them to HandBrake.
- **[[entities/plex]]** and **[[entities/jellyfin]]** – Media‑server platforms that stream the HandBrake‑encoded files throughout the home network.
- **[[concepts/disc_ripping]]** – The broader process of converting physical media to digital files, of which HandBrake is a key encoding step.

---

## Practical Tips (from the session)
- Choose HandBrake presets that match your playback hardware (e.g., TV, phone).
- Keep at least two backups of the encoded library to avoid data loss.
- Periodically revisit encoding settings as newer HandBrake releases may improve quality or compression.
