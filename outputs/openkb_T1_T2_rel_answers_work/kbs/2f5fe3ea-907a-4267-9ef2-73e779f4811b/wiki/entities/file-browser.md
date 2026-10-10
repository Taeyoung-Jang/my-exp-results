---
sources: ["summaries/session-37_2025-02-15.md"]
type: "Product"
description: "File Browser is a lightweight, single‑binary web file manager for self‑hosted use."
---

## File Browser (product)

File Browser is a minimal, single‑binary web‑based file manager that can run on a low‑power home server such as a Raspberry Pi or mini‑PC.  In the context of [[summaries/session-37_2025-02-15]] it is recommended as the preferred web UI for a Syncthing‑based personal hub because it:

- Provides a clean, browser‑friendly interface for browsing files on the LAN.
- Supports read‑only mode, which matches the low‑maintenance, mostly‑view‑only workflow described.
- Runs with minimal resource usage, fitting the goal of a [[concepts/self-hosted-home-hub]].

File Browser pairs well with other components mentioned in the session:

- **Sync layer** – Syncthing handles peer‑to‑peer file synchronization across devices ([[concepts/cross-device-syncing]], [[concepts/low-maintenance-file-sync]]).
- **Remote access** – When accessing the hub from outside the home network, a VPN such as Tailscale or WireGuard is preferred, keeping the File Browser service behind the VPN rather than exposing HTTPS directly.
- **Notes** – The file manager can serve plain Markdown files, which can then be viewed or edited with lightweight browsers like StackEdit or Editor.md, or rendered via static‑site generators such as mdbook or mkdocs.

Overall, File Browser fulfills the requirement for a simple, low‑maintenance web UI that complements the self‑hosted, secure, and device‑agnostic setup outlined in the session.
