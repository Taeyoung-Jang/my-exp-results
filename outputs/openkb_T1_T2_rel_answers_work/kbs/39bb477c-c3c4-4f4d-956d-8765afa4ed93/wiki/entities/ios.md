---
sources: ["summaries/session-33_2025-02-14.md"]
type: "Product"
description: "Apple's mobile operating system for iPhone and iPad."
---

# iOS

**Type:** product

**Description:** Apple’s mobile operating system that powers the iPhone and iPad.

## Role in Session 33

In the conversation *[[summaries/session-33_2025-02-14]]*, iOS is the platform on which the user wants to implement a **browser‑first phone** strategy. The assistant recommends several iOS‑specific settings to reduce app clutter and background activity:
- Turning off **Background App Refresh** (Settings → General → Background App Refresh).
- Disabling **Siri suggestions** (Settings → Siri & Search).
- Trimming notifications to only essential communication apps.
- Setting location permissions to “While Using the App.”

These tweaks are framed as part of the broader [[concepts/app-clutter-management]] and [[concepts/minimal-iphone-setup]] approaches.

## Recommended Native Apps on iOS

The minimal iPhone setup suggested in the session keeps only those apps that integrate tightly with iOS system services:
- [[entities/apple-messages]] (Messages)
- Phone (built‑in)
- [[entities/facetime]] (FaceTime)
- [[entities/apple-maps]] (Maps)
- Camera & Photos (built‑in)
- [[entities/apple-wallet]] (Wallet)
- Settings (built‑in)
- App Store – [[entities/app-store]]
- A 2FA solution (either a [[entities/authenticator-app]] or, preferably, [[concepts/passkey-authentication]] via iCloud Keychain)
- Optional: a music/podcast player, Files or Notes (e.g., [[entities/apple-notes]])

All other services are recommended to be accessed through **Safari** shortcuts, leveraging the iOS home‑screen organization concept [[concepts/iphone-home-screen-organization]].

## Security & 2FA on iOS

For a strict “no extra apps” policy, the session highlights two iOS‑friendly authentication methods:
- **Passkeys** – built into iOS via iCloud Keychain, aligning with [[concepts/passkey-authentication]].
- **Hardware security keys** – such as a YubiKey, which work without installing additional software.

If a passkey‑compatible service is unavailable, a traditional [[entities/authenticator-app]] can be used, though it adds an extra app to the device.

## Related Entities & Concepts

- [[entities/apple]] – the company behind iOS.
- [[entities/iphone]] – the primary hardware platform for iOS.
- [[entities/safari]] – the web browser used for the browser‑first approach.
- [[entities/icloud]] – provides the passkey infrastructure.
- [[entities/hardware-security-key]] – an alternative 2FA method.
- [[concepts/browser-first-phone]] – the overall strategy discussed.

---

*This page captures the iOS‑specific recommendations and context from the session‑33 discussion.*