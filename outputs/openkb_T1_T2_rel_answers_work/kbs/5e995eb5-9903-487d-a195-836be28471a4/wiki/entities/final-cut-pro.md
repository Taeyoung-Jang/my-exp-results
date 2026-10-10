---
sources: ["summaries/session-37_2024-06-15.md"]
type: "Product"
description: "Apple's professional video editing application for macOS."
---

# Final Cut Pro

**Type:** product  
**Description:** Apple’s flagship non‑linear editing (NLE) software for macOS.

## Overview
Final Cut Pro (FCP) is Apple’s flagship non‑linear editing (NLE) software, used for high‑resolution, multi‑camera projects and known for its magnetic timeline, optimised performance on macOS, and robust media management tools.

## Mentions in [[summaries/session-37_2024-06-15]]
In the discussion about organizing large multi‑camera, effects‑heavy edits, the assistant noted that the workflow tips (clear naming, bin structure, adjustment layers, nesting, and proxy usage) apply equally to **Premiere**, **DaVinci Resolve**, and *Final Cut Pro*. Although the conversation did not dive into product‑specific UI details, the same principles of [[concepts/folder-bin-mirroring]], [[concepts/adjustment-layer-strategy]], [[concepts/proxy-workflow]] and [[concepts/series-template-workflow]] can be applied when using Final Cut Pro.

## Related Concepts
- [[concepts/folder-bin-mirroring]] – mirroring disk folders with project bins.
- [[concepts/adjustment-layer-strategy]] – using adjustment layers for global effects.
- [[concepts/proxy-workflow]] – creating low‑resolution proxies for smoother playback.
- [[concepts/series-template-workflow]] – reusing a master project template across episodes.

## Related Entities
- [[entities/adobe-premiere-pro]] – comparable NLE mentioned in the same discussion.
- [[entities/davinci-resolve]] – another NLE covered alongside Final Cut Pro.

## Practical Tips for FCP Users
- Replicate the folder‑to‑bin layout described in the session to keep media organized.
- Use compound clips (the FCP equivalent of nesting) for locked sections of a timeline.
- Leverage proxy media (optimized media in FCP) when editing 4 K multicam footage.
- Create adjustment layers (via adjustment clips) for global colour grading or effects, mirroring the [[concepts/adjustment-layer-strategy]].