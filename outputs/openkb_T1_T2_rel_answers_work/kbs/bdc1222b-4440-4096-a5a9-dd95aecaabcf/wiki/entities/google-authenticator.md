---
sources: ["summaries/session-33_2025-02-13.md", "summaries/session-15_2024-06-15.md"]
type: "Product"
description: "Google Authenticator is a 2FA app generating time‑based codes for accounts."
---

# Google Authenticator (product)

Google Authenticator is a two‑factor authentication (2FA) app that creates time‑based one‑time passwords (TOTP) for securing Google and other online accounts.

## Key facts from **[[summaries/session-15_2024-06-15]]**
- **Manual transfer required**: The app does **not** participate in the standard [[concepts/google_backup]] process. Users must use the built‑in *Transfer accounts* feature to export a QR code before moving to a new device.
- **Common migration gotcha**: Assuming Google backs up Authenticator data leads to being locked out of 2FA‑protected services after a device wipe.
- **Backup codes**: The document advises saving backup/recovery codes for every account that uses Authenticator, as a safety net.
- **Step in migration checklist**: On day one, prepare the Authenticator export, then after the new Pixel 9 restores other data, complete the import and verify a few codes work.

## Related concepts and entities
- [[concepts/google_backup]] – explains why Authenticator needs a separate export step.
- [[entities/google]] – the company behind the app.
- [[entities/google-authenticator]] – self‑reference for consistency with the wiki structure.
- [[entities/google-messages]] – another Google service mentioned in the migration guide.
- [[entities/signal]] – an alternative messaging app with its own transfer method, contrasted with Authenticator’s manual export.

## Usage tips for a smooth transition
1. Open **Google Authenticator** on the old phone → *Transfer accounts* → *Export accounts* → generate QR code.
2. Keep the old phone on and powered while you set up the new device.
3. After the new phone finishes the system restore, open Authenticator, choose *Import accounts*, and scan the QR code.
4. Test several accounts to ensure codes are valid.
5. Store backup/recovery codes in a secure password manager.

Following these steps avoids the typical pitfall of losing access to 2FA‑protected accounts during a phone migration.

See also: [[summaries/session-33_2025-02-13]]