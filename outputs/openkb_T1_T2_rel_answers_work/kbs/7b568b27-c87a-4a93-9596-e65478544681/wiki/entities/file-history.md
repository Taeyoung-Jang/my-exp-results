---
sources: ["summaries/session-11_2025-06-15.md"]
type: "Product"
description: "Built‑in Windows 11 feature that continuously backs up user files with versioning"
---

# File History

**Type:** Product  
**Description:** Built‑in Windows 11 feature that continuously backs up user files and keeps previous versions.

**Key facts from [[summaries/session-11_2025-06-15]]:**
- Used as **Drive A** in the recommended two‑layer backup strategy.
- Configured to back up user folders automatically, retaining unlimited versions.
- Provides rapid recovery from accidental deletion or ransomware‑encrypted files.
- Works together with a periodic system image created by [[entities/windows-backup-restore]] on an external drive ([[entities/external-drive]]).

**Related concepts:**
- [[concepts/two-layer-backup]]
- [[concepts/versioning]]
- [[concepts/local-file-organization]]

**Typical setup on [[entities/windows-11]]:**
1. Enable File History in Settings → Update & Security → Backup.
2. Choose an always‑connected external drive (e.g., [[entities/external-drive]]) as the backup destination.
3. Set “Keep saved versions” to “Forever” and the frequency to the shortest interval.

**Benefits:** Low‑maintenance, continuous protection, searchable version history, integrates with the broader backup plan described in the session summary.