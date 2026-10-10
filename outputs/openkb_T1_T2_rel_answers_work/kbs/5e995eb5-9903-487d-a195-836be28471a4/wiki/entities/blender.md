---
sources: ["summaries/session-15_2023-06-15.md"]
type: "Product"
description: "Free open‑source 3D creation suite recommended for low‑end video editing workflows."
---

# Blender

Blender is a free, open‑source 3D creation suite used for modeling, animation, rendering, and compositing. In the **session‑15_2023‑06‑15** discussion, Blender was suggested as the go‑to tool for basic 3‑D work on an older Windows 10 machine with limited CPU, RAM, and GPU resources.

## Key points from the session
- **Lightweight rendering**: Use the **Eevee** real‑time engine for previews and keep **Cycles** samples very low, enabling denoising to maintain acceptable quality on weak hardware.
- **Modest export resolution**: Render 3‑D elements at a modest resolution (e.g., 720p) and upscale later if needed, aligning with the overall [[concepts/proxy-workflow]] for video editing.
- **Integration with low‑end video editing**: Blender complements the recommended low‑end video editing stack (e.g., [[entities/kdenlive]] or [[entities/shotcut]]) by providing simple 3‑D assets without overwhelming system resources.
- **Performance considerations**: The advice to keep other system tweaks (see [[concepts/windows-performance-tweaks]]) such as closing background apps and using an SSD for caches also benefits Blender’s responsiveness.

## Related tools and concepts
- **Proxy workflow**: The session emphasizes using proxies for video; Blender’s output can be fed into the same proxy pipeline.
- **HandBrake conversion**: Before importing phone footage into the video editor, the user is advised to convert VFR clips with [[entities/handbrake]] to a constant frame rate, ensuring sync with any 3‑D overlays.
- **MediaInfo verification**: After rendering, [[entities/mediainfo]] can be used to confirm that the exported video matches the desired frame rate and codec.

## Reference
- This information is drawn from the summary of the conversation: [[summaries/session-15_2023-06-15]].