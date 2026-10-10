---
type: "Concept"
sources: ["summaries/session-33_2025-02-14.md"]
description: "Guidelines for a lean iPhone configuration focusing on essential native apps and browser shortcuts."
---

# Minimal iPhone Setup

A **minimal iPhone setup** is a systematic approach to keeping an iPhone fast, low‑maintenance, and functional by limiting installed native apps to those that genuinely benefit from deep system integration, while handling the rest via Safari home‑screen shortcuts. The concept ties together [[concepts/app-clutter-management]], [[concepts/browser-first-phone]], and [[concepts/iphone-home-screen-organization]] and is illustrated in [[summaries/session-33_2025-02-14]].

## Core Native Apps (≈10‑15)
| Category | Typical Apps | Rationale |
|----------|--------------|-----------|
| Communication | [[entities/apple-messages]], Phone, FaceTime, iMessage | Direct access to SMS, iMessage, and telephony is faster and more reliable than web equivalents. |
| Navigation & Location | [[entities/apple-maps]] | Uses device GPS and offline maps more efficiently than a browser map. |
| Media Capture | Camera, Photos | System‑level integration (Live Photos, HDR) cannot be matched in a browser. |
| Payments & Identity | [[entities/apple-wallet]], 2FA authenticator (or passkeys) | Secure element access and Apple Pay require native support. |
| System Utilities | Settings, App Store, Files, Notes (iCloud sync) | Core OS functions and iCloud syncing are built‑in. |
| Optional Essentials | Preferred email client, Music/Podcast player | Retained only if used frequently; otherwise shift to web. |

## Categories Better Served as Safari Shortcuts
- Social media (Twitter, Instagram, etc.)
- Shopping & e‑commerce sites
- News and content aggregators
- Banking portals (except for push alerts)
- Video streaming platforms
- General reference, note‑dumping, task lists

Creating home‑screen shortcuts in [[entities/safari]] gives an app‑like feel without consuming storage or background resources. This aligns with the [[concepts/browser-first-phone]] mindset.

## iOS Settings Tweaks
1. **Background App Refresh** – `Settings → General → Background App Refresh`. Turn it off globally or per‑app for non‑essential apps.
2. **Siri Suggestions** – `Settings → Siri & Search`. Disable top‑level suggestions and the “Learn from this App” toggle for each non‑essential app.
3. **Notifications** – Keep only communication, calendar, and essential alerts. Disable banners, badges, and sounds for the rest.
4. **Location Permissions** – Set most apps to *While Using the App*.
5. **Battery Optimization** – Review battery usage in `Settings → Battery` and restrict background activity where possible.

These adjustments reduce background processing while preserving the functionality of the core apps.

## 2FA Strategy for a Strict Minimal Setup
- **Passkeys** (via [[entities/icloud]]) – No extra app needed; works natively in Safari. Preferred for sites that support them.
- **Hardware Security Key** – Physical device (e.g., YubiKey) provides strong authentication without installing an app.
- **Authenticator App** – Viable but violates the minimal‑apps principle; keep only if required.
- **SMS Codes** – Universally available but less secure and can be noisy.

For a browser‑first workflow, the recommended combo is **passkeys** as the primary method, supplemented by a **hardware security key** for sites lacking passkey support.

---
*Related concepts*: [[concepts/app-clutter-management]], [[concepts/browser-first-phone]], [[concepts/iphone-home-screen-organization]], [[concepts/passkey-authentication]]
