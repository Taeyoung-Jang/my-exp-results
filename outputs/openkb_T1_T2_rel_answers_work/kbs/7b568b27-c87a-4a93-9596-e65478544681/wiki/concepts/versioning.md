---
type: "Concept"
sources: ["summaries/session-34_2025-09-15.md", "summaries/session-11_2025-06-15.md"]
description: "Versioning keeps multiple historical copies of files for easy recovery."
---

# Versioning

Versioning is the practice of preserving successive snapshots of a file or set of files so that earlier states can be restored when needed.  It protects against accidental deletion, unwanted edits, and malicious changes such as ransomware encryption.

## Why versioning matters
- **Accidental loss** – If a file is mistakenly overwritten or deleted, a prior version can be recovered.
- **Ransomware mitigation** – Offline backups combined with versioned copies let you roll back to a clean state without paying a ransom.
- **Change tracking** – Having a history of edits makes it easy to compare revisions and understand the evolution of a document or project.

## Implementation in the "session‑11_2025‑06‑15" setup
- **Drive A (primary backup)** uses **File History** on [[entities/windows-11]] to automatically capture every change in user folders.  The tool retains versions indefinitely, giving fine‑grained recovery points.
- **Drive B (offline safeguard)** stores a periodic full system image created with [[entities/windows-backup-restore]].  While this image is not a continuous versioning system, it provides a boot‑recoverable snapshot that complements the continuous versioning of Drive A.
- Both drives are typical [[entities/external-drive]]s; the second can be a [[entities/home-nas]] for added redundancy.

## Relationship to other concepts
- Versioning is a core component of [[concepts/two-layer-backup]], enabling the primary layer (continuous versioning) and the secondary layer (offline full‑image snapshots) to work together.
- It supports a [[concepts/local-file-organization]] strategy by ensuring that even a simple, search‑driven folder layout remains safe over time.

## Reference
- See the full summary of the source discussion in [[summaries/session-11_2025-06-15]].

See also: [[summaries/session-34_2025-09-15]]