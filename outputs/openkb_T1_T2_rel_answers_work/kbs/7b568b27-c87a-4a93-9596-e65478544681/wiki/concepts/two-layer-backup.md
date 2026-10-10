---
type: "Concept"
sources: ["summaries/session-34_2025-09-15.md", "summaries/session-11_2025-06-15.md"]
description: "A backup strategy using a continuously connected primary drive plus an offline secondary copy."
---

## Two‑Layer Backup

**Definition**: A backup strategy that combines a continuously connected primary backup drive with an offline secondary backup drive (or NAS) to provide redundancy, versioning, and protection against ransomware while requiring minimal user intervention.

**Why it matters** – By pairing an always‑on backup with an isolated copy, you guard against both accidental deletion and catastrophic events such as drive failure or ransomware infection.

### Primary layer (Drive A)
- Always attached to the computer.
- Uses [[entities/file-history]] on [[entities/windows-11]] to back up user folders automatically.
- Provides [[concepts/versioning]] and quick recovery from accidental deletions or malicious modifications.
- Typically an [[entities/external-drive]] kept plugged in.

### Secondary layer (Drive B)
- Kept unplugged or on a separate network location (e.g., a [[entities/home-nas]]) most of the time.
- Created with [[entities/windows-backup-restore]] to produce a full system image on a weekly (or bi‑weekly) schedule.
- Acts as a “cold” mirror that is immune to ransomware that might affect the primary drive.

### Operational cadence
- **Drive A** runs unattended, updating at the shortest interval allowed by File History (often hourly).
- **Drive B** is connected once a week (or every two weeks) to run the system‑image backup, then disconnected.

### Benefits
- **Redundancy**: failure of the internal drive or Drive A can be recovered from Drive B.
- **Versioning**: daily changes are tracked by File History.
- **Low maintenance**: only occasional plugging of Drive B and occasional inbox cleanup.
- **Compatibility with simple organization**: works well with a [[concepts/local-file-organization]] that relies on search rather than deep folder hierarchies.

### Reference
- This concept is illustrated in the discussion from [[summaries/session-11_2025-06-15]].

See also: [[summaries/session-34_2025-09-15]]