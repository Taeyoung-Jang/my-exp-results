---
sources: ["summaries/session-33_2025-02-14.md"]
type: "Product"
description: "A physical authentication device that provides push‑free two‑factor login."
---

# Hardware Security Key

A **hardware security key** is a small physical device (often USB‑C, Lightning, or NFC) that provides secure, password‑less authentication for online services. It is used as a second factor in two‑factor authentication (2FA) and can replace software authenticator apps.

## Relevance to a Minimal iPhone Setup
- In the context of the **browser‑first phone** approach described in [[summaries/session-33_2025-02-14]], a hardware security key is recommended as the “next cleanest” 2FA method after passkeys because it requires **no installed app** and generates no background notifications.
- It fits the [[concepts/minimal-iphone-setup]] philosophy by keeping the device free of extra apps while still offering strong security for logins that do not yet support [[concepts/passkey-authentication]].
- When paired with iOS, a hardware key works with services that support the FIDO2/WebAuthn standard, allowing the user to authenticate directly from Safari without needing an authenticator app.

## How It Interacts with iOS Settings
- No need to enable **Background App Refresh** for a hardware key, as it operates only when physically tapped.
- Since it does not generate push notifications, it does not interfere with the trimmed notification settings recommended for a minimal iPhone (see [[concepts/app-clutter-management]]). 

## Comparative Advantages
| Feature | Hardware Security Key | Authenticator App | SMS Codes | Passkeys |
|---------|----------------------|-------------------|-----------|----------|
| Requires install? | No | Yes | No | No (built‑in) |
| Works in Safari? | Yes (WebAuthn) | No (requires app) | Yes (via SMS) | Yes |
| Physical presence needed? | Yes (tap) | No | No | No |
| Security level | High (phishing‑resistant) | Medium | Low | High |

## Related Entities and Concepts
- [[entities/ios]] – the operating system where the hardware key is used.
- [[entities/iphone]] – the device type discussed in the minimal setup.
- [[entities/safari]] – the browser that can leverage the key via WebAuthn.
- [[concepts/browser-first-phone]] – the broader strategy that motivates using a hardware key.
- [[concepts/app-clutter-management]] – the overall goal of reducing unnecessary apps.

## References
- Session discussion where the hardware security key is suggested as the preferred 2FA method for a strict minimal‑app approach: [[summaries/session-33_2025-02-14]].