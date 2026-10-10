---
type: "Concept"
sources: ["summaries/session-36_2024-12-15.md"]
description: "A minimal, human‑readable hierarchy for long‑term personal archives."
---

# Folder Structure

**Type:** Concept

**Description:** A simple, scalable directory layout that keeps personal digital archives understandable and resilient over decades.

---

## Overview
The folder structure recommended in [[summaries/session-36_2024-12-15]] focuses on a small set of top‑level categories that are easy to navigate without special software. Each category is organized chronologically where appropriate, and project work is kept in a stable, self‑contained location.

---

## Top‑Level Categories
```
Archive/
├─ Documents/
├─ Photos/
├─ Video/
├─ Audio/
├─ Projects/
└─ Personal Notes/
``` 
- **Documents, Photos, Video, Audio, Personal Notes**: Contain content sorted by *year* (e.g., `Photos/2026/2026‑03‑Trip‑to‑Japan`).
- **Projects**: Holds a permanent slug for each project (e.g., `Projects/project‑aurora/`). Inside each project, time‑based subfolders (`2024‑notes`, `2025‑drafts`, …) capture chronological material while the project root stores non‑time‑bound assets like a README, final outputs, or scripts.

---

## Naming Conventions
Files that benefit from a date use the pattern `YYYY‑MM‑DD‑keyword‑description.ext`. This ensures natural sorting and immediate context without opening the file. Non‑date files receive clear, descriptive names (e.g., `README.md`).

---

## Interaction with Other Concepts
- The structure works hand‑in‑hand with [[concepts/open-formats]] by encouraging formats that embed their own metadata (e.g., EXIF for images, front‑matter for Markdown). 
- A well‑defined hierarchy simplifies backup planning; see [[concepts/backup-strategy]] for a recommended 3‑2‑1 approach that mirrors the same directory layout.

---

## Benefits
1. **Future‑proof readability** – Anyone can understand the layout years later.
2. **Minimal maintenance** – Few top‑level folders reduce the chance of accidental re‑organization.
3. **Scalable for long‑running projects** – Projects stay in a single home, avoiding link rot and duplication.
4. **Facilitates automated backups** – Consistent paths make scripting and versioning straightforward.

---

## Implementation Tips
- Create the top‑level `Archive` folder once and never rename it.
- Stick to the prescribed category names; avoid ad‑hoc additions.
- When a new year begins, simply add a new subfolder under the relevant category.
- For each project, draft a concise `README.md` at the root that describes the project, the purpose of each year folder, and high‑level milestones.

---

*This concept page synthesizes the guidance from [[summaries/session-36_2024-12-15]] into a reusable reference for building durable personal archives.*