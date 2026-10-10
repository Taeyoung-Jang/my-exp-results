---
sources: ["summaries/session-37_2025-10-14.md"]
type: "Product"
description: "Bitwarden is a cross‑platform password manager that syncs vaults via its own cloud service."
---

# Bitwarden

Bitwarden is a **password manager** that stores encrypted vaults in the cloud and syncs them across devices.  It is frequently recommended for users who keep a **local Windows** account because it provides password sync without tying into the Windows login system.

## Key points from [[summaries/session-37_2025-10-14]]
- Works independently of a [[entities/microsoft-account]]; you keep a purely local [[entities/windows-11]] login.
- Stores passwords in an encrypted vault (see [[concepts/encryption]]) and syncs through Bitwarden’s own cloud infrastructure, avoiding reliance on Microsoft’s cloud services.
- Does **not** attempt to replace or integrate with the Windows credential store, preserving the stability of a local account.
- Can be paired with a secure note to store a [[entities/bitlocker]] recovery key, giving a convenient but still private location for that critical data.

## Related concepts
- [[concepts/password-manager]] – the broader category of tools that manage and sync passwords.
- [[concepts/encryption]] – how Bitwarden protects vault data.

## Typical usage in the discussed setup
1. Install Bitwarden on Windows 11.
2. Log in with a Bitwarden account (or self‑hosted instance) to enable vault sync.
3. Use the vault for cross‑device password access while keeping the Windows login local.
4. Optionally store BitLocker recovery keys or other sensitive notes in the secure notes section.

Bitwarden therefore fits the recommendation to “layer on just enough cloud” for password convenience while maintaining a private, stable local Windows environment.