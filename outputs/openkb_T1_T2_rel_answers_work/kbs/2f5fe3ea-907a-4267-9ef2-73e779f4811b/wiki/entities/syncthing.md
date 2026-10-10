---
sources: ["summaries/session-37_2025-02-15.md"]
type: "Product"
description: "A peer-to‑peer file synchronization tool for personal devices."
---

# Syncthing

**Type**: Product

Syncthing is an open‑source, peer‑to‑peer file synchronization program that lets multiple devices keep folders in sync without a central server. It runs on low‑power hardware such as a Raspberry Pi or a mini‑PC and requires only occasional updates, making it ideal for a **low‑maintenance** personal hub.

---

## Highlights from [[summaries/session-37_2025-02-15]]
- Recommended as the **simplest** solution for a private home file hub when the goal is minimal upkeep.
- Works out‑of‑the‑box for **cross‑device syncing** across laptops, phones, and a always‑on home server.
- Operates over encrypted connections and does not depend on any commercial cloud provider.
- Pairs well with a lightweight web file browser such as [[entities/file-browser]] for LAN access.
- For remote access, combine Syncthing with a VPN like [[entities/tailscale]] or [[entities/wireguard]] rather than exposing a public HTTPS endpoint.

---

## Related Concepts
- [[concepts/low-maintenance-file-sync]] – Syncthing exemplifies a setup that “just works” after initial configuration.
- [[concepts/self-hosted-home-hub]] – It is a core component for building a personal, self‑hosted hub.
- [[concepts/cross-device-syncing]] – Provides seamless file replication across multiple devices.

---

## Related Entities
- [[entities/file-browser]] – Often used as the simple web UI to view files synced by Syncthing.
- [[entities/tailscale]] and [[entities/wireguard]] – Preferred VPN solutions for secure remote access to the Syncthing server.
- [[entities/nextcloud]] – Mentioned as a more feature‑rich alternative when a full ecosystem is desired.

---

## Quick Start Tips
1. Install Syncthing on each device (Linux, Windows, macOS, Android, iOS).
2. Create a shared folder on the home server and add the same folder on client devices.
3. Set the folder to **read‑only** on devices where you only need browsing access.
4. Use a VPN (Tailscale or WireGuard) to reach the home server from outside the LAN.
5. Optionally, run a lightweight web UI like File Browser to browse files in a browser.

---

*Syncthing remains a lightweight, secure, and mostly hands‑off solution for personal file and note synchronization.*