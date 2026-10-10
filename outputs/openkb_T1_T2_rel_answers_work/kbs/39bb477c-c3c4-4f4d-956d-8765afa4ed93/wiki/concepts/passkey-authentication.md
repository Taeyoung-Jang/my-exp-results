---
type: "Concept"
sources: ["summaries/session-33_2025-02-14.md"]
description: "Passwordless, biometric login using iCloud Keychain on iOS devices."
---

# Passkey Authentication

**Definition**: Passkey authentication is a password‑less, public‑key‑based login method that leverages the device’s secure enclave and iCloud Keychain to authenticate users with biometrics (Face ID/Touch ID) or device PIN.

---

## Overview
Passkeys replace traditional passwords and one‑time codes with cryptographic key pairs stored locally on the device. The private key never leaves the device, while the public key is shared with the service during registration. Authentication is performed by proving possession of the private key, which is unlocked by a biometric check or device passcode.

## How it works on iPhone
1. **Creation** – When a website or app supports passkeys, iOS (via [[entities/ios]]) prompts the user to create a passkey, storing the private key in the secure enclave and syncing it via [[entities/icloud]].
2. **Login** – On a subsequent login, the user selects the stored passkey in Safari or a native app, authenticates with Face ID/Touch ID, and the device signs a challenge with the private key.
3. **Verification** – The service verifies the signature using the public key, granting access without any password entry.

## Advantages for a Minimal iPhone Setup
- **No extra app required** – Passkeys are managed by the operating system, fitting the [[concepts/minimal-iphone-setup]] strategy of keeping only essential native apps.
- **Reduced background activity** – Since the authentication flow is handled by iOS, there’s no need for background sync or network traffic from a separate authenticator app, aligning with [[concepts/app-clutter-management]].
- **Higher security** – Private keys are hardware‑protected and never transmitted, mitigating phishing and credential‑reuse risks.
- **Seamless browser‑first experience** – Works directly in Safari, supporting a [[concepts/browser-first-phone]] workflow where most services are accessed via web shortcuts.

## Comparison with Other 2FA Methods
| Method | App Needed? | Works in Safari? | Security | User Experience |
|--------|-------------|-------------------|----------|-----------------|
| Passkey | No (system‑level) | ✅ | Very high (hardware‑bound keys) | Fast, biometric only |
| Hardware security key | No (plug‑in) | Limited (WebAuthn on Safari) | Very high | Requires physical key |
| Authenticator app | Yes (e.g., [[entities/authenticator-app]]) | No (code generation only) | High | Manual code entry |
| SMS | No | ✅ | Low (SIM swap attacks) | Text message codes |

## Implementation Tips for iPhone Users
- Ensure **iCloud Keychain** is enabled: `Settings → Apple ID → iCloud → Keychain`.
- Use **Safari’s built‑in passkey prompt** when visiting a supporting site.
- For services lacking passkey support, consider a **[[entities/hardware-security-key]]** as a secondary method to stay within a low‑app footprint.
- Keep **Background App Refresh** disabled for unnecessary apps (see [[concepts/app-clutter-management]]) to maintain a lean system.

---

## Related Concepts
- [[concepts/app-clutter-management]] – Managing app bloat and background processes.
- [[concepts/browser-first-phone]] – Using web shortcuts instead of native apps.
- [[concepts/minimal-iphone-setup]] – Choosing essential native apps for iPhone.

## Source
- Summary of recommendations from [[summaries/session-33_2025-02-14]].