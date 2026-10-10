---
type: "Concept"
sources: ["summaries/session-39_2025-06-15.md"]
description: "A workflow that limits active heavy apps to keep low‑spec devices responsive."
---

## Lightweight Workflow

**Definition**: A set of practices that keep only one resource‑intensive application active at a time, using the browser as a central hub and off‑loading or suspending other tools to preserve system responsiveness on compact machines.

### Core Principles
1. **Single heavy‑process focus** – Keep either the browser (with essential tabs) or a single document/editor open; treat all other tools as short‑lived tasks.
2. **Browser‑centric hub** – Pin frequently used tabs, close or bookmark the rest, and use a tab‑manager extension to suspend inactive tabs.
3. **Web‑first for productivity apps** – Prefer web versions of Google Docs, Sheets, and Slack to reduce RAM usage compared to desktop clients.
4. **Selective notifications** – Limit Slack (or similar communication tools) to mentions/DMs only, and run it in a dedicated Chrome window to benefit from background throttling.
5. **Automatic tab discarding** – Configure extensions like Auto Tab Discard to pause tabs after 15‑20 minutes, while whitelisting critical sites (Slack, Google Docs/Sheets, Meet) to avoid losing work.

### Practices from Session‑39
- **Pin essential tabs** and use a reading list or bookmarks for the rest (see [[summaries/session-39_2025-06-15]]).
- **Use Chrome’s Memory Saver** and disable background apps to further cut resource drain.
- **Run Slack in the browser** with notifications limited to mentions and direct messages, keeping it in its own window to leverage Chrome’s background throttling.
- **Choose a lightweight editor** and close unused project windows, allowing quick re‑opens without memory cost.

### Related Concepts
- [[concepts/resource-management]] – broader strategies for efficient CPU/RAM use.
- [[concepts/tab-management]] – tools and settings to suspend or group tabs.
- slack notification optimisation – (not in whitelist, described without brackets) focuses on minimal Slack impact.
- chrome performance tuning – (not in whitelist, described without brackets) covers Chrome settings that aid lightweight workflows.

### Benefits
- Maintains snappy performance on a **local workstation** with limited RAM.
- Reduces the need for costly **cloud‑compute** or GPU instances for everyday tasks.
- Lowers energy consumption and extends battery life.

---
*Page compiled from insights in [[summaries/session-39_2025-06-15]].*