---
type: "Concept"
sources: ["summaries/session-37_2024-06-15.md"]
description: "A repeatable workflow using a master project to seed bins, assets, and routing for each episode."
---

# Series Template Workflow

**Definition** – A repeatable project‑level structure that creates a master "Series_Template" project containing all reusable bins, assets, and routing presets, then duplicates it for each new episode (e.g., EP01, EP02). This ensures consistent folder‑to‑bin mirroring, naming conventions, and asset handling across a series.

---

## Core Elements

1. **Master Project (Series_Template)**
   - Holds top‑level bins: *Footage, Audio, Graphics, Timelines* and a dedicated *SeriesAssets* bin for lower thirds, captions, Fusion titles, and audio bus presets.
   - Mirrors the on‑disk folder hierarchy (see [[concepts/folder-bin-mirroring]]).  
   - Designed to be duplicated, not edited in‑place for each episode.

2. **Duplication Process**
   - In DaVinci Resolve (or other NLE), use **Project Manager → Duplicate**.
   - Rename the copy to the episode identifier (e.g., `EP01`, `EP02`).
   - The duplicated project inherits the exact bin layout, track routing, and preset configurations.

3. **Naming Conventions**
   - Timelines: `EP01_Main`, `EP01_Interview_MC01`, etc.
   - Exports: `EP01_Main_v03_1080pReview` or `EP01_Final_MasterProRes`.
   - Multicam clips: `MC_A‑B‑C` or `MC_Interview01`.
   - These patterns keep the series searchable and version‑controlled.

4. **Asset Management**
   - **Reusable graphics** (lower thirds, logos) live in *SeriesAssets* and can be stored in **Power Bins** if live updates across episodes are required.
   - Audio routing presets (buses, track assignments) are also saved in the master project, ensuring each episode starts with the same mix hierarchy.

5. **Updating the Template**
   - **Freeze old episodes** – Do not retroactively apply template changes to finished projects unless a full remaster is needed.
   - **Evolve forward** – Modify the master template for new assets or routing changes; subsequent episode duplicates inherit the updates.
   - **Selective retro‑fit** – When a change must affect older episodes, import the updated assets or copy‑paste the relevant settings from the updated template into the old project.

## When to Use Power Bins vs. Template Duplication
| Asset Type | Recommended Approach |
|------------|----------------------|
| Graphics that rarely change (e.g., fixed lower‑third designs) | Store in *SeriesAssets* within the duplicated project.
| Assets that evolve frequently (new lower‑third version, updated caption style) | Place in **Power Bins** so they are centrally editable and instantly available in all open projects.
| Audio bus routing or preset configurations | Keep inside the master template; duplicate per episode to keep routing consistent.

## Benefits
- **Consistency** – Every episode starts with identical bin structure and naming, reducing confusion.
- **Scalability** – Adding new episodes is a single click, no manual recreation of folders or bins.
- **Version control** – Clear timeline and export naming makes locating the latest cut trivial.
- **Efficiency** – Minimal repetitive setup time; focus shifts to creative editing.

---

## Related Concepts
- [[concepts/folder-bin-mirroring]] – The underlying principle of mirroring disk folders to NLE bins.
- [[concepts/adjustment-layer-strategy]] – Often combined with this workflow to apply global looks via adjustment layers.

---

## Source
- Summarized from [[summaries/session-37_2024-06-15]].