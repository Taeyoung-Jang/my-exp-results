---
sources: ["summaries/session-39_2025-06-15.md"]
type: "Product"
description: "Auto Tab Discard is a Chrome extension that automatically suspends inactive tabs to save memory."
---

## Auto Tab Discard

**Type:** Product

Auto Tab Discard is a Chrome extension designed to improve system responsiveness on low‑spec machines by automatically discarding (suspending) inactive browser tabs. In the conversation documented in [[summaries/session-39_2025-06-15]], it was recommended as the preferred tab‑management tool for users who keep 30–60 tabs open.

### Key Facts from the Session
- **Primary use case:** Automatically puts inactive tabs to sleep after about 15–20 minutes of inactivity, freeing RAM while allowing instant wake‑up when the tab is re‑selected.
- **Whitelist strategy:** Critical sites such as Slack, Google Docs, Google Sheets, and Google Meet should be added to the extension’s whitelist to prevent discarding mid‑task, especially when forms or meetings are in progress.
- **Interaction with Chrome:** Works best when Chrome’s built‑in *Memory Saver* is also enabled and when the setting *Continue running background apps when Chrome is closed* is disabled. The extension respects Chrome’s background‑window throttling, making it a low‑overhead solution for a [[entities/local-workstation]] or any compact ultrabook.
- **Comparison:** Compared to [[entities/tab-session-manager]], Auto Tab Discard offers a hands‑off approach that continuously manages memory, whereas Tab Session Manager requires manual grouping of tab sets.

### Related Concepts
- [[concepts/tab-management]] – the broader practice of controlling tab count and resource usage.
- [[concepts/resource-management]] – the overall strategy of minimizing simultaneous heavy processes.
- [[concepts/lightweight-workflow]] – the workflow philosophy of keeping only one heavyweight application active at a time.

### Related Entities
- [[entities/chrome]] – the browser platform where Auto Tab Discard operates.
- [[entities/slack]] – an example of a whitelisted web app that benefits from the extension’s selective discarding.

---
*This entity page aggregates information from the session‑39 discussion and links to relevant concepts and entities within the wiki.*