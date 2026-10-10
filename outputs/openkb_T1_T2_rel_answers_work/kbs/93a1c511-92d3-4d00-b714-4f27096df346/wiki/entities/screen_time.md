---
sources: ["summaries/session-34_2024-06-15.md"]
type: "Product"
description: "iOS feature for monitoring and limiting device usage"
---

## Screen Time

**Type:** Product (built‑in iOS feature)

### Overview
Screen Time is Apple’s native tool for tracking device usage and enforcing usage limits on iOS devices. It resides in *Settings → Screen Time* and provides granular controls such as App Limits, Downtime, and passcode protection.

### Key Features
- **App Limits:** Set daily time allowances for specific apps or categories.
- **Downtime:** Schedule periods when only selected apps are usable.
- **Passcode Protection:** Prevent immediate overrides by requiring a Screen Time passcode.
- **Notification Management:** Turn off notifications for restricted apps to reduce pull.

### Usage in [[summaries/session-34_2024-06-15]]
The conversation outlines a “set‑and‑forget” workflow for weekday social‑media restriction:
1. Open **Settings → Screen Time → App Limits**.
2. Add a limit for chosen social apps, set to a minimal allowance (e.g., 1 minute).
3. Use **Customize Days** to disable the limit on Saturday and Sunday, keeping weekdays restricted.
4. In **Screen Time → Downtime**, schedule a weekday evening block and ensure the apps are not listed under *Always Allowed*.
5. Set a Screen Time passcode that is hard to guess in the moment (optionally delegated to a trusted friend).
6. Move the apps off the home screen and disable their notifications for added friction.

These steps embody the concepts of [[concepts/gentle_defaults]], [[concepts/fractional_friction]], and [[concepts/offline_anchors]] by turning boundaries into default system settings, introducing small obstacles, and pairing online time with phone‑free periods.

### Related Concepts
- [[concepts/gentle_defaults]]
- [[concepts/fractional_friction]]
- [[concepts/offline_anchors]]

### Related Entities
- [[entities/apple]] – the company that develops iOS and Screen Time.
- [[entities/iphone]] – the primary device where Screen Time is used.

### References
- Session 34 (2024‑06‑15) discussion on practical digital‑boundary setup using Screen Time.