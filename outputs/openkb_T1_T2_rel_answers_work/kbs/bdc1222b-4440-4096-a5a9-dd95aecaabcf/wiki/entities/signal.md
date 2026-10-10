---
sources: ["summaries/session-15_2024-06-15.md"]
type: "Product"
description: "Signal is a secure messaging app with end‑to‑end encrypted chats."
---

# Signal (product)

Signal is a cross‑platform, end‑to‑end encrypted messaging application focused on privacy and security.

## Role in the session‑15 migration advice
- The assistant recommends **keeping Signal installed on the old Android phone** because Signal does **not** back up chats to Google Drive; it requires a **direct device‑to‑device transfer** during the new phone setup.
- Failing to perform this transfer before wiping the old device is noted as a common gotcha that can lead to permanent loss of chat history.

## Backup and restore considerations
- **No Google backup**: Unlike many Android apps, Signal does not integrate with [[concepts/google_backup]].
- **Transfer method**: Use Signal’s built‑in “Transfer account” feature, which generates a QR code on the old phone and scans it on the new device. This moves encrypted chat history locally.
- **Verification step**: After the transfer, open Signal on the new phone and confirm that recent conversations appear before resetting the old device.

## Recommendations from the document
1. **Keep the old phone powered on** throughout the migration process.
2. Initiate the Signal transfer **after** the Pixel 9’s initial system restore but **before** wiping the old phone.
3. Confirm chats are present on the new device before the final factory reset.

## Related entities and concepts
- Platform: [[entities/android]]
- Ecosystem context: [[entities/google]] (the broader Google‑centric Android environment) 
- Migration checklist reference: [[summaries/session-15_2024-06-15]]
- Long‑term support considerations: [[concepts/long_term_phone_support]]

---
*Signal’s unique backup approach makes it a special case in Android phone migrations, requiring manual transfer rather than relying on cloud services.*