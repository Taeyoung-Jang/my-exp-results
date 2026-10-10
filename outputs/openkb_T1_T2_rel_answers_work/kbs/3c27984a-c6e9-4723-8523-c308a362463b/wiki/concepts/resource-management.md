---
type: "Concept"
sources: ["summaries/session-39_2025-06-15.md"]
description: "Techniques for minimizing resource use on low‑spec machines while staying productive."
---

# Resource Management

**Definition**: Strategies and settings that reduce CPU, memory, and I/O load on a device, allowing essential tools to stay responsive without sacrificing functionality.

## Core Principles (from [[summaries/session-39_2025-06-15]])
1. **Limit simultaneous heavy processes** – Keep only one “heavy” app (browser, document, or editor) active at a time.
2. **Leverage the browser as a hub** – Pin essential tabs, close or bookmark the rest, and use a tab‑manager to suspend idle tabs.
3. **Prefer lightweight versions** – Use web‑based Google Docs/Sheets instead of desktop clients, and run Slack in the browser rather than the standalone app.
4. **Use targeted notifications** – Enable only mentions/DMs in Slack to avoid constant background polling.
5. **Apply OS and browser performance tweaks** – Disable background apps in Chrome, enable Memory Saver, and whitelist critical sites.

## Practical Techniques
- **Tab Management**: Install a tab‑suspension extension such as [[entities/auto-tab-discard]] (or the alternative [[entities/tab-session-manager]]) and set a discard timer of 15‑20 minutes. Whitelist sites like Slack, Google Docs, Google Sheets, and Google Meet to prevent loss of in‑progress work.
- **Chrome Optimisation**: Turn off *Continue running background apps when Chrome is closed*, enable *Memory Saver*, and add essential URLs to the *Always keep these sites active* list.
- **Slack Configuration**: Use the web client in its own Chrome window, enable notifications only for mentions and direct messages, and disable channel‑wide alerts.
- **Document Handling**: Keep a single document open at a time in the browser; close additional tabs when switching tasks.
- **Editor Choice**: Select a lightweight editor and close unused project windows.

## Related Concepts
- [[concepts/lightweight-workflow]] – complementary approach focusing on minimal‑impact tool selection.
- [[concepts/tab-management]] – detailed practices for handling many open tabs.
- slack notification optimisation – (not in whitelist, mentioned here as plain text) specific Slack notification tuning.
- chrome performance tuning – (plain text) Chrome settings that enhance responsiveness.

## Why It Matters
Effective resource management extends the usable lifespan of a **[[entities/local-workstation]]**, prevents productivity loss due to lag, and reduces the hidden cost of hardware upgrades or cloud‑compute rentals.

---
*This concept page synthesizes guidance from the session‑39 discussion and can be applied broadly to low‑spec computing environments.*