---
type: "Concept"
sources: ["summaries/session-37_2024-06-15.md"]
description: "Using adjustment layers for global effects to keep timelines tidy and editable."
---

# Adjustment‑Layer Strategy

**Definition**: An adjustment‑layer strategy is the practice of applying effects, color grades, or corrections to an adjustment layer instead of individual clips, so that the effect can be toggled, edited, or removed globally across a stretch of the timeline.

---

## Why use adjustment layers?
- **Maintain readability** – A single layer replaces dozens of duplicated per‑clip effects, keeping the track list clean.
- **Fast toggling** – Turn the layer on/off to compare rough versus polished looks without re‑rendering each clip.
- **Version control** – Adjustments can be renamed or versioned (e.g., `Adj_Look_v01`) and nested like any other clip.
- **Consistent rendering** – Most NLEs (e.g., [[entities/adobe-premiere-pro]], [[entities/davinci-resolve]], [[entities/final-cut-pro]]) treat adjustment layers as lightweight overlays, reducing playback strain.

---

## When to apply an adjustment layer (from [[summaries/session-37_2024-06-15]])
| Use‑case | Recommended approach |
|----------|----------------------|
| Global colour grade or creative look | Place a colour‑correction adjustment layer over the entire sequence or a major segment.
| Light noise reduction, sharpening, or exposure lifts that affect many shots | Apply a single adjustment layer instead of adding the same effect to each clip.
| Temporary rough‑cut look (e.g., low‑resolution proxy grading) | Use an adjustment layer that can be disabled when switching to high‑resolution proxies.
| Per‑clip unique issues (e.g., a single over‑exposed shot) | **Do not** use an adjustment layer; apply the effect directly to that clip.

---

## Implementation steps
1. **Create the layer** – In the timeline, add a new adjustment layer (Premiere: *File → New → Adjustment Layer*; Resolve: *Effects Library → Adjustment Clip*).
2. **Name it descriptively** – e.g., `Adj_GlobalLook_v01`.
3. **Apply desired effects** – colour grading, noise reduction, LUTs, etc.
4. **Position it** – Stretch the layer to cover the intended range (entire timeline, a scene, or a multicam section).
5. **Nest if needed** – When a segment becomes complex, nest it together with its adjustment layer to keep the main timeline tidy.

---

## Interaction with other concepts
- Works hand‑in‑hand with [[concepts/folder-bin-mirroring]]: keeping assets organized on disk mirrors the logical grouping of adjustment layers in the timeline.
- Complementary to a [[concepts/series-template-workflow]]: a series template can include pre‑configured adjustment layers for a consistent look across episodes.
- For low‑end hardware, adjustment layers are lighter than per‑clip effects, aligning with best practices in [[concepts/low-end-video-editing]] and [[concepts/proxy-workflow]].

---

## Cross‑NLE considerations
- **Premiere Pro** – Adjustment layers inherit all effect parameters of the clips beneath them.
- **DaVinci Resolve** – Use *Adjustment Clip*; some colour‑specific nodes may need to be placed on the clip instead of the layer.
- **Final Cut Pro** – Apply effects to a *Connected Clip* above the primary storyline to achieve the same result.

---

*By adopting an adjustment‑layer strategy, editors can keep large, effect‑heavy projects organized, improve playback performance, and simplify future revisions.*