---
sources: ["summaries/session-37_2025-02-15.md"]
type: "Product"
description: "Tailscale is a zero‑config VPN service that simplifies secure remote access."
---

# Tailscale (product)

Tailscale is a cloud‑managed mesh VPN that creates a secure, peer‑to‑peer network between devices with minimal configuration. It is often recommended for personal self‑hosted setups because it provides encrypted connectivity without the need to expose services directly to the internet.

## Key facts from [[summaries/session-37_2025-02-15]]
- **Purpose**: Used as the preferred remote‑access method for a low‑maintenance home hub.
- **Advantages**: Eliminates the need for manual port forwarding, certificate management, and complex firewall rules.
- **Integration**: Works alongside [[entities/syncthing]] for file sync and can replace or complement other VPN solutions like [[entities/wireguard]].

## Relevant concepts
- [[concepts/self-hosted-home-hub]] – the broader scenario where Tailscale provides secure remote connectivity.
- [[concepts/low-maintenance-file-sync]] – the goal of keeping the overall system simple and hands‑off.
- [[concepts/cross-device-syncing]] – Tailscale enables devices to communicate securely, facilitating cross‑device sync performed by tools such as Syncthing.

## Typical usage pattern
1. Install the Tailscale client on each device (desktop, laptop, phone, Raspberry Pi, etc.).
2. Log in with a supported identity provider; devices automatically join the same virtual network.
3. Access services (e.g., a lightweight web file browser) via their local network addresses over the Tailscale network.

## Comparison with alternatives
- **WireGuard**: Tailscale builds on WireGuard but adds automatic key exchange, device discovery, and an easy‑to‑use control plane, reducing operational overhead.
- **Direct HTTPS exposure**: Tailscale avoids the increased attack surface and certificate upkeep associated with publicly exposed HTTPS endpoints.

## Resources
- Official website: https://tailscale.com
- Documentation for setting up a home server with Tailscale.
