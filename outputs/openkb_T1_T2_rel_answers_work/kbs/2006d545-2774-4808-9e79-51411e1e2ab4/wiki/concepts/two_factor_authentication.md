---
type: "Concept"
sources: ["summaries/session-06_2024-06-15.md"]
description: "Two‑Factor Authentication adds a second verification step to secure online accounts."
---

## Two‑Factor Authentication

Two‑Factor Authentication (2FA) is a security mechanism that requires users to provide two separate forms of identification before gaining access to an account.  It builds on the traditional username/password model by adding a second factor, which can be something the user **has** (a device or token) or something the user **is** (biometrics).  The goal is to reduce the risk of unauthorized access even if the primary password is compromised.

### Core Factors
- **Knowledge** – something the user knows (e.g., a password or PIN).
- **Possession** – something the user has, such as an authenticator app, a hardware security key, or a mobile phone capable of receiving SMS codes.
- **Inherence** – something the user is, typically a biometric characteristic like a fingerprint or facial recognition.

### 2FA Methods Highlighted in Session 06
| Method | Privacy Impact | Security Strength | Convenience |
|--------|----------------|-------------------|-------------|
| Authenticator app (e.g., Google Authenticator, Authy) | Low – no personal info shared | High – time‑based one‑time passwords (TOTP) are resistant to phishing | Moderate – requires a smartphone but no extra hardware |
| Hardware security key (U2F/YubiKey) | Very low – no personal data transmitted | Very high – cryptographic challenge‑response, immune to phishing | Low – must carry the key and manage backups |
| SMS‑based codes | High – reveals personal phone number to the service | Medium – vulnerable to SIM‑swap and SS7 attacks | High – works on any phone that can receive texts |

The session "[[summaries/session-06_2024-06-15]]" recommends using authenticator apps as the sweet spot between privacy and security, and hardware keys as the strongest option when convenience permits.  SMS‑based 2FA is considered a fallback for services that do not support other methods; the document advises mitigating its risks with a dedicated secondary SIM and backup codes.

### Trade‑offs and Considerations
1. **Convenience vs. Security** – Stronger factors (hardware keys) often require extra effort to carry and configure, while weaker factors (SMS) are more user‑friendly but expose personal data and are vulnerable to carrier‑level attacks.
2. **Recovery Planning** – Users should store recovery codes securely (e.g., in a password manager) and, when possible, enable multiple 2FA methods on the same account to avoid lock‑out.
3. **Privacy Concerns** – Providing a phone number (especially a primary personal number) can link the account to a real identity.  A secondary SIM, as discussed in [[concepts/secondary_sim_management]], helps separate the verification channel from the user's main identity.

### Best Practices (derived from the source)
- Prefer authenticator apps or hardware keys over SMS where supported.
- If SMS is required, use a dedicated, low‑cost secondary SIM that stays active to avoid number recycling.
- Secure the carrier account with a strong PIN and limit exposure of the phone number.
- Keep backup codes in a secure password manager and consider adding an additional 2FA factor for redundancy.

### Related Concepts
- [[concepts/online_privacy]] – broader strategies for minimizing personal data exposure online.
- [[concepts/secondary_sim_management]] – detailed guidance on maintaining a secondary SIM used for SMS 2FA.
