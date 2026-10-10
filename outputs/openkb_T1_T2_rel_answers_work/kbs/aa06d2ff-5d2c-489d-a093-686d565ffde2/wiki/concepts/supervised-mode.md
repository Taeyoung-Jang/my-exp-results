---
type: "Concept"
sources: ["summaries/session-39_2024-12-13.md"]
description: "iOS supervised mode is a device‑wide MDM state that enforces restrictions while allowing limited UI actions."
---

# Supervised Mode (iOS)

**Definition**

Supervised Mode on iOS refers to a management state applied by an organization's Mobile Device Management (MDM) system that gives the IT department full control over the device. In this state the device is *supervised* – the MDM can enforce security policies, restrict app removal, and push managed apps directly to the home screen.

**Key Characteristics**
- **Device‑wide control** – Unlike a simple work profile, supervision applies to the entire device, not just a container of apps.
- **Restricted UI actions** – Users cannot delete or hide managed (gray placeholder) icons, though they can often drag them.
- **Automatic app placement** – New managed apps appear on the first available home‑screen page; iOS provides no toggle to stop this.
- **Visibility of management** – The status is shown under **Settings → General → VPN & Device Management** as “managed and supervised.”

**Implications for Home‑Screen Organization**

Even under supervision, users can still rearrange icons:
1. Long‑press an icon to enter edit mode.
2. Drag managed icons into a folder or to the rightmost home‑screen page.
3. The leftmost page remains the default home screen, so placing personal apps there keeps them front‑and‑center.

These steps are described in detail in [[summaries/session-39_2024-12-13]] and rely on the broader concept of [[concepts/home-screen-organization]].

**Interaction with Mobile Device Management**

Supervised Mode is a specific configuration of [[concepts/mobile-device-management]]. It allows IT to:
- Push apps silently.
- Enforce security settings (passcode, encryption, etc.).
- Control updates and configuration profiles.

Because the supervision is device‑wide, users cannot opt‑out of new managed apps; they must manually move them after they appear.

**Related Entities**
- [[entities/ios]] – The operating system where supervised mode is applied.
- [[entities/iphone]] – Typical hardware that may be enrolled in supervised mode.
- [[entities/it-department]] – The organizational group that configures and maintains the supervision.

**Practical Tips**
- Verify supervision status via **Settings → General → VPN & Device Management**.
- Use a dedicated folder (sometimes called a *staging folder*) to collect all managed icons on the last home‑screen page.
- There is currently no iOS setting to automatically route new managed apps into that folder; manual relocation is required.

**See Also**
- [[concepts/mobile-device-management]]
- [[concepts/home-screen-organization]]
- [[concepts/supervised-mode]] (self‑reference for taxonomy)
