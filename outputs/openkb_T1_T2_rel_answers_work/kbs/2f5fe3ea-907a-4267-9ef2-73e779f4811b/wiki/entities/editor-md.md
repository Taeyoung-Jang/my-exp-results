---
sources: ["summaries/session-37_2025-02-15.md"]
type: "Product"
description: "A lightweight self‑hosted browser Markdown editor."
---

# Editor.md

Editor.md is an open‑source, browser‑based **Markdown editor** that can be self‑hosted with minimal configuration. It provides a clean editing interface, live preview, and supports common Markdown extensions.

## Key facts from [[summaries/session-37_2025-02-15]]
- Recommended in the session as a **low‑maintenance** option for editing notes stored as plain Markdown files.
- Presented as an alternative to the heavier [[entities/nextcloud]] stack and to other browser editors like [[entities/stackedit]].
- Fits naturally into a **self‑hosted home hub** setup that uses [[entities/syncthing]] for file synchronization and a lightweight web file browser such as [[entities/file-browser]].
- Works well with static‑site generators (e.g., [[entities/mdbook]] or [[entities/mkdocs]]) to render notes for read‑only browsing.

## Related concepts
- [[concepts/self-hosted-home-hub]] – the overall approach of keeping files and notes on a personal server.
- [[concepts/low-maintenance-file-sync]] – using tools like Syncthing to keep data in sync with minimal upkeep.
- [[concepts/client-side-search]] – can be combined with static‑site generators to enable fast, client‑side searching of Markdown notes.

## Usage scenario
1. Store notes as plain Markdown files in a synced folder managed by [[entities/syncthing]].
2. Serve the folder via a simple web server (e.g., File Browser) for LAN access.
3. Edit or view notes directly in the browser using Editor.md, optionally pairing it with a static‑site generator for richer navigation.

## Advantages
- No database or heavy backend required.
- Simple deployment: a single HTML/JS bundle.
- Works offline and integrates smoothly with existing sync solutions.

---
*This page aggregates the information about Editor.md as mentioned in the session‑37 discussion.*