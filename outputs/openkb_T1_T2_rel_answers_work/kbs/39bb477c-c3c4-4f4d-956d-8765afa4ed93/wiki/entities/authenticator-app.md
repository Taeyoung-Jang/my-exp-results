---
sources: ["summaries/session-33_2025-02-14.md"]
type: "Product"
description: "A mobile app that generates time‑based one‑time passwords for two‑factor authentication."
---

# Authenticator App

**Type:** Product  
**Description:** Mobile applications that generate time‑based one‑time passwords (TOTP) for two‑factor authentication (2FA).

## Role in minimal iPhone discussions
In [[summaries/session-33_2025-02-14]] the Authenticator App is evaluated as a **non‑essential** app for a “browser‑first” iPhone setup. While it provides strong 2FA, keeping it installed violates the [[concepts/minimal-iphone-setup]] principle of limiting native apps to those that integrate tightly with the operating system.

## Alternatives highlighted
The conversation recommends using [[concepts/passkey-authentication]] (built‑in iCloud Keychain) or a [[entities/hardware-security-key]] as lower‑maintenance replacements. SMS codes are mentioned as an alternative but noted for weaker security.

## Interaction with iOS settings
If an Authenticator App is retained, it should be excluded from background activity via **Settings → General → Background App Refresh** and limited in notifications to avoid unnecessary alerts, aligning with the [[concepts/app-clutter-management]] approach.

## Related entities
- [[entities/ios]]
- [[entities/iphone]]
- [[entities/icloud]]
- [[entities/safari]] (used for browser‑first workflows)
