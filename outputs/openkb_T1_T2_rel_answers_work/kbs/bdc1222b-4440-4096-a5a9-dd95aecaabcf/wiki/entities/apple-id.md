---
sources: ["summaries/session-33_2025-02-13.md"]
type: "Product"
description: "Apple ID is Apple’s unified account for iCloud, App Store, and other services."
---

# Apple ID

**Type:** Product

Apple ID is the central credential that lets users access Apple’s ecosystem, including iCloud, the App Store, iMessage, FaceTime, and device activation.

---

## Key Security Features (from [[summaries/session-33_2025-02-13]])
- **Strong, unique password** – recommended to use a password manager.
- **Two‑Factor Authentication (2FA)** – enabled via the **Sign‑In & Security** settings on macOS and iPadOS.
- **Trusted phone numbers** – can add multiple numbers to avoid lock‑out when a number changes.
- **Account Recovery options** – choose between a **recovery contact** or a **recovery key**.

These aspects are covered in the concept page [[concepts/apple-id-security]].

---

## Recovery Options
- **Recovery contact** – a trusted person who can provide a verification code during a lock‑out flow. See [[entities/recovery-contact]].
- **Recovery key** – a 28‑character code that can unlock the account if 2FA devices are unavailable. See [[entities/recovery-key]].

The trade‑offs between these options are discussed in [[concepts/account-recovery-options]].

---

## iCloud Sync & Encryption
Apple ID controls which data categories sync to iCloud (Photos, Keychain, Notes, etc.) and ensures they are end‑to‑end encrypted. For details on the sync and encryption model, see [[concepts/icloud-sync-encryption]] and the related entity [[entities/icloud]].

---

## Device Management
Through the Apple ID settings on macOS and iPadOS, users can view and remove devices linked to the account, helping to keep the ecosystem secure.

---

## Related Platforms
- **iOS** devices use the same Apple ID for seamless continuity. See [[entities/ios]].

---

## References
- Session summary: [[summaries/session-33_2025-02-13]]
