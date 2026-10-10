---
sources: ["summaries/session-37_2025-02-15.md"]
type: "Product"
description: "WireGuard is a lightweight, modern VPN solution for secure remote network access."
---

## WireGuard (product)

WireGuard is an open‑source, high‑performance VPN protocol and software implementation designed for simplicity, speed, and strong cryptography. It creates encrypted point‑to‑point connections that can be used to securely access home‑hosted services from anywhere on the internet.

### Role in the **self‑hosted home hub** setup
In the discussion of session‑37 (2025‑02‑15), WireGuard was recommended as the preferred method for remote access to a personal file‑sync hub. Compared with exposing HTTPS directly, WireGuard (often deployed via the **Tailscale** service) reduces the attack surface by keeping services behind a private network, eliminating the need to manage public certificates or firewall rules.

### Complementary tools
- Works well alongside [[entities/syncthing]] for **cross‑device syncing** of files and notes.
- Often paired with [[entities/tailscale]] for an easy‑to‑configure, cloud‑managed WireGuard network.

### Benefits highlighted
- **Low maintenance**: Once set up, the tunnel requires little ongoing care, fitting the goal of a low‑maintenance file sync hub.
- **Strong security**: Utilises modern cryptographic primitives and runs in the kernel for minimal overhead.
- **Cross‑device capability**: Enables seamless access from laptops, phones, and tablets, supporting the [[concepts/cross-device-syncing]] workflow.

### Related concepts
- [[concepts/self-hosted-home-hub]] – the overall architecture the VPN secures.
- [[concepts/low-maintenance-file-sync]] – the broader aim of keeping the system simple and reliable.

### Reference
For the original recommendation and context, see [[summaries/session-37_2025-02-15]].