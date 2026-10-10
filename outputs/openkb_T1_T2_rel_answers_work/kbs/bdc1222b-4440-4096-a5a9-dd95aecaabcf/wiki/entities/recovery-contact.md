---
sources: ["summaries/session-33_2025-02-13.md"]
type: "Other"
description: "A trusted person added to an Apple ID to assist with verification during account recovery."
---

# Recovery Contact

**What it is**
A *recovery contact* is a person you designate in your Apple ID settings who can provide a short verification code if you ever get locked out of your account. The contact does **not** gain access to your data; they only help confirm your identity during the recovery flow.

**Key facts from [[summaries/session-33_2025-02-13]]**
- Added via **Settings → Your Name → Sign‑In & Security → Account Recovery** on both macOS and iPadOS.
- The contact sees your name under **Account Recovery** in their own Apple ID settings (iPhone/iPad: Settings → Their Name → Sign‑In & Security → Account Recovery; Mac: System Settings → Their Name → Sign‑In & Security → Account Recovery).
- When you need help, they open that screen, tap your name, and Apple generates a short verification code for them to read to you.
- Recommended for most users because it is low‑risk and easy to change, unlike a [[entities/recovery-key]].

**Why use a recovery contact?**
- Provides a safety net if your trusted phone number changes or you lose access to a device.
- Avoids the pitfalls of a recovery key, which is powerful but unforgiving if lost.
- Works in conjunction with other [[concepts/apple-id-security]] measures such as a strong password and two‑factor authentication.

**How it relates to other concepts**
- Part of the broader [[concepts/account-recovery-options]] view, which includes both recovery contacts and recovery keys.
- Complements [[concepts/icloud-sync-encryption]] by ensuring you can regain access to encrypted iCloud data without compromising security.

**Interaction with other entities**
- Requires an existing [[entities/apple-id]] for the user and the designated contact.
- May be used alongside a [[entities/recovery-key]] for an even stronger (but more complex) recovery strategy.

**Best practice summary**
1. Keep your trusted phone numbers up‑to‑date (see [[concepts/long_term_phone_support]] for guidance on maintaining contact methods).
2. Add at least one recovery contact you truly trust.
3. Periodically verify that the contact sees your name in their Account Recovery screen.
4. Consider a recovery key only if you have a secure, permanent storage method.

**Further reading**
- Detailed step‑by‑step checklist in [[summaries/session-33_2025-02-13]].