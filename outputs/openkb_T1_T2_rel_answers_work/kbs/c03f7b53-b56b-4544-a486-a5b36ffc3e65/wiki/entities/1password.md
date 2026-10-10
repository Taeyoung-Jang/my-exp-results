---
sources: ["summaries/session-37_2025-10-14.md"]
type: "Product"
description: "1Password is a cross‑platform password manager offering cloud‑synced vaults."
---

# 1Password

**Type:** Product

1Password is a commercial password‑manager service that stores passwords, secure notes, and other secrets in an encrypted vault that syncs across devices via the provider’s cloud infrastructure. It is designed to operate independently of the operating system’s login mechanisms, making it suitable for users who keep a **local** Windows account while still wanting seamless password access on multiple devices.

## Key points from [[summaries/session-37_2025-10-14]]
- Recommended in the Windows 11 checklist as a **standalone password manager** that does **not** take over the Windows credential store.
- Provides cloud‑based sync of the vault, allowing cross‑device password availability without tying the sync to a Microsoft account.
- Works well alongside a local‑only Windows login, preserving privacy and system stability.
- Mentioned alongside alternatives such as [[entities/bitwarden]] and [[entities/keepassxc]].

## Related concepts and entities
- [[concepts/password-manager]] – the broader category of tools for managing credentials.
- [[entities/windows-11]] – the operating system version discussed in the checklist.
- [[entities/microsoft-account]] – contrasted with 1Password for users avoiding cloud‑linked Windows accounts.

## Typical usage scenario
1. Install 1Password on the Windows 11 machine.
2. Create a master password for the vault; this password never leaves the device unencrypted.
3. Sign into the 1Password cloud service to enable vault sync across phones, tablets, and other computers.
4. Use the 1Password browser extension or desktop app to fill credentials without integrating with the Windows credential manager.

## Security notes
- The vault is encrypted end‑to‑end; the provider never sees the plaintext data.
- Users should store the master password securely, as loss of it means loss of access to all stored secrets.
- When using BitLocker on a local account, keep the BitLocker recovery key in a secure location, such as a 1Password secure note, to avoid being locked out after hardware changes.
