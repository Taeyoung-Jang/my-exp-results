---
type: "Concept"
sources: ["summaries/session-37_2025-02-15.md"]
description: "A personal, low‑maintenance server for syncing files and notes across devices without relying on commercial cloud services."
---

# Self‑Hosted Home Hub

**Definition**: A self‑hosted home hub is a small, always‑on server (e.g., Raspberry Pi or mini‑PC) that provides private file storage, synchronization, and note access for a household, reachable from any device on the LAN or via a secure remote‑access method.

## Core Characteristics
| Aspect | Typical Implementation |
|--------|-----------------------|
| **Hardware** | Low‑power single‑board computer or inexpensive mini‑PC running continuously. |
| **File Sync** | Peer‑to‑peer sync using [[entities/syncthing]], which keeps files identical across phones, laptops, and the hub without a central cloud. |
| **Web UI** | Lightweight file browsers such as [[entities/file-browser]] or minimal servers like *miniserve* for read‑only navigation. |
| **Notes** | Plain Markdown files stored in the synced folder; edited/viewed with browser‑based editors like [[entities/stackedit]] or [[entities/editor-md]]. |
| **Remote Access** | Secure VPN (e.g., [[entities/tailscale]] or [[entities/wireguard]]) preferred over exposing HTTPS directly, reducing attack surface. |
| **Maintenance** | Single‑binary services, occasional updates, automatic backups; no complex database or heavy web stack. |

## Benefits
- **Independence**: No lock‑in to commercial cloud providers; data stays on‑premises.
- **Security**: Controlled by the owner, with optional VPN tunnel for external access.
- **Low Overhead**: Minimal CPU/RAM usage; easy to set up on existing hardware.
- **Scalability**: Adding new devices is as simple as installing the sync client.

## Typical Workflow (derived from [[summaries/session-37_2025-02-15]])
1. Install Syncthing on the hub and each client device.
2. Place files and Markdown notes in a shared folder that Syncthing replicates.
3. Run a lightweight web file browser (e.g., File Browser) on the hub for LAN access.
4. For remote use, connect via Tailscale or WireGuard VPN.
5. Optionally generate a static site from the notes using [[entities/mdbook]] or [[entities/mkdocs]] for richer browsing and client‑side search.

## Related Concepts
- [[concepts/low-maintenance-file-sync]] – focuses on the sync component of a home hub.
- [[concepts/cross-device-syncing]] – broader view of keeping data consistent across many devices.
- [[concepts/client-side-search]] – often paired with static‑site generators to enable quick note lookup.
- [[concepts/self-hosted-home-hub]] – this very concept, providing the overarching framework.

---
*This page synthesizes the recommendations from the session‑37 discussion and serves as a reference for building a personal home hub.*