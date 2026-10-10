---
type: "Concept"
sources: ["summaries/session-37_2024-06-15.md"]
description: "Mirroring project folder structure to NLE bins to keep media organized and relinkable."
---

# Folder‑to‑Bin Mirroring

**Definition** – A workflow practice where the on‑disk folder hierarchy of a video project is duplicated exactly as bin (or smart bin) hierarchy inside the non‑linear editor (NLE). This one‑to‑one mapping ensures that assets are easy to locate, relink, and manage across editing sessions.

## Why use it?
- **Predictable navigation** – Editors can jump from the file explorer to the corresponding bin without guessing where a clip lives.
- **Robust relinking** – If media moves on disk, the matching bin structure makes it straightforward to re‑point the NLE to the new location.
- **Cross‑project consistency** – A standard layout can be reused for every episode or video, reducing setup time.
- **Scalability** – Works equally well for small edits and large multi‑camera, effects‑heavy productions like those described in [[summaries/session-37_2024-06-15]].

## Typical folder & bin layout
```
ProjectName/
├─ Footage
│   ├─ A‑Cam
│   ├─ B‑Cam
│   ├─ C‑Cam
│   ├─ ScreenRecords
│   └─ Other
├─ Audio
│   ├─ VO
│   ├─ Music
│   └─ SFX
├─ Graphics
│   ├─ LowerThirds
│   ├─ Logos
│   └─ Templates
├─ Exports
│   ├─ Review
│   └─ Final
└─ ProjectFiles
    ├─ Premiere_or_Resolve
    └─ Autosaves
```
Create NLE bins with the **exact same names** and nesting order (e.g., a bin called *Footage* containing sub‑bins *A‑Cam*, *B‑Cam*, etc.).

## Implementation steps
1. **Plan the folder tree** before importing any media.
2. **Create matching bins** in the NLE (Premiere, DaVinci Resolve, or Final Cut).
3. **Import media** into the appropriate bin directly from its disk folder; most editors will preserve the folder name as the bin name.
4. **Maintain naming conventions** for clips (e.g., `A001_C003_interviewWide`) so the relationship stays clear.
5. **Lock the structure** – avoid ad‑hoc bin creation later; instead, add sub‑bins only if they match a new folder.

## Interaction with other concepts
- Works hand‑in‑hand with [[concepts/adjustment-layer-strategy]]: once bins are tidy, applying global adjustment layers becomes faster because the editor can quickly locate the relevant clips.
- Supports the [[concepts/series-template-workflow]] in Resolve, where a master project’s bin layout can be duplicated for each episode, preserving the folder‑to‑bin mirroring across the series.

## Best‑practice tips
- Prefix top‑level bins with numbers (e.g., `00_Admin`, `01_Timelines`) to keep them at the top of the bin list.
- Keep versioned timelines (`EP01_Main_v01`, `v02`, …) in a dedicated *Timelines* bin.
- Regularly **autosave** the project file inside the *ProjectFiles* folder to keep everything together.

By adopting folder‑to‑bin mirroring, editors gain a reliable, scalable foundation for any project size, from quick low‑end cuts to high‑resolution multi‑camera productions.