---
sources: ["summaries/session-39_2024-12-13.md"]
type: "Product"
description: "iOS is Apple's mobile operating system used on iPhone and iPad devices."
---

# iOS

**Type:** Product

**Overview**

iOS is the proprietary mobile operating system developed by Apple Inc. for its line of smartphones and tablets, including the [[entities/iphone]]. It provides the core user interface, app ecosystem, and security framework for these devices.

**MDM and Supervision**

When a device is enrolled in [[concepts/mobile-device-management]] by an [[entities/it-department]], it can be placed into a *supervised* state. In this mode, the settings under **Settings → General → VPN & Device Management** indicate that the device is *managed and supervised*, allowing the organization to enforce policies such as app installation restrictions and home‑screen layout control. This is described in the context of [[concepts/supervised-mode]].

**Home‑Screen Organization**

The document **[[summaries/session-39_2024-12-13]]** outlines practical steps for reorganizing the iOS home screen under supervision:
- Long‑press any icon to enter edit mode.
- Create a folder (or use an existing one) and drag all gray, restricted placeholders into it.
- Move the folder to the far‑rightmost home‑screen page so the leftmost page remains personal.
- iOS does not provide a setting to automatically prevent newly pushed managed apps from appearing on the first page; users must manually relocate them.

These actions relate directly to the concept of [[concepts/home-screen-organization]], which covers strategies for arranging app icons and pages.

**Limitations**

- No built‑in iOS toggle exists to stop new managed apps from auto‑appearing on the home screen.
- The App Library cannot block supervised apps from showing on active pages; it only assists in post‑move organization.

**Interaction with Other Platforms**

While iOS relies on the supervised mode for strict control, Android devices can use a *Work Profile* to isolate managed apps from personal ones. The document references both platforms, contrasting iOS's single‑profile approach with Android's optional work‑profile separation.

**Related Entities**

- [[entities/android]] – Android operating system, which offers a Work Profile for separation.
- [[entities/smartphone]] – General category of mobile devices that include iOS devices.

**Reference**

For a detailed checklist and discussion of iOS home‑screen cleanup under MDM supervision, see **[[summaries/session-39_2024-12-13]]**.