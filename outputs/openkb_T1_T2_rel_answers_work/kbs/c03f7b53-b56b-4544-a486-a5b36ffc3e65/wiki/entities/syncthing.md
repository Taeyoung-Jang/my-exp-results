---
sources: ["summaries/session-37_2025-10-14.md"]
type: "Product"
description: "Syncthing is a peer‑to‑peer file synchronization product."
---

# Syncthing (product)

Syncthing is an open‑source, peer‑to‑peer file synchronization **product** that lets devices sync selected folders directly over the internet or a local network without needing a centralized cloud service.

## Role in the backup strategy (session‑37)
- In the **session‑37** checklist, Syncthing is recommended as a way to create an *offsite backup* of important personal files (documents, photos, work folders) while keeping the Windows login **local**.  
- It operates independently of the Windows credential system, allowing users to sync specific folders to a home server or another trusted device.
- This aligns with the broader [[concepts/offsite-backup]] approach, providing redundancy without attaching the entire system identity to a cloud provider.

## Interaction with other tools
- Syncthing can complement the **system‑image backup** method (see [[concepts/system-image-backup]]) by handling continuous, folder‑level sync of user data.
- It serves as an alternative to commercial cloud‑sync services, fitting into a *privacy‑first* backup plan where the user retains full control over the storage location.

## Security considerations
- Since Syncthing works over encrypted TLS connections, it provides **encryption** in transit, relevant to [[concepts/encryption]].
- Users are responsible for securing the destination device (e.g., enabling BitLocker on external drives) and storing any recovery keys safely (see [[entities/bitlocker]] and [[entities/tpm]]).

## Related concepts and entities
- [[concepts/backup-strategy]] – overarching approach that includes both local system images and offsite folder sync.
- [[entities/windows-11]] – the operating system context for the recommended setup.
- [[entities/keepassxc]] and [[entities/bitwarden]] – password manager options mentioned alongside Syncthing for secure credential storage.
- [[summaries/session-37_2025-10-14]] – source document where Syncthing is discussed as part of the checklist.
