---
type: "Concept"
sources: ["summaries/session-12_2024-06-15.md"]
description: "Comparison of cloud storage and external drives for digital asset management."
---

# Cloud Storage vs. External Drive

**What it is** – A decision framework that weighs the strengths and weaknesses of using cloud storage versus an external hard drive (or a hybrid of both) for organizing, protecting, and accessing personal digital assets.

---

## Overview
Cloud storage provides *any‑where access* and acts as a *safety net* because data lives off‑site, while an external drive offers *fast local access*, a *one‑time cost*, and full ownership of the data. Most users benefit from a hybrid approach, designating one medium as the **source of truth** and the other as a backup snapshot.

---

## Key Advantages
| Aspect | Cloud Storage | External Drive |
|--------|---------------|----------------|
| Accessibility | Access from any device with internet | Only when the drive is connected |
| Cost model | Subscription‑based, scalable | Up‑front purchase, limited capacity |
| Data loss risk | Protected against local hardware failure | Vulnerable to physical failure, theft, or damage |
| Control | Managed by provider, may have account lockouts | Full user control, no third‑party lock‑in |

---

## Common Pitfalls
- **Over‑reliance on a single solution** – hard‑drive failure is more common than expected; cloud accounts can be locked or become costly.
- **Duplicate or messy folder structures** – arises when both locations are treated as independent masters. Choose one direction for organization (usually cloud → drive).
- **Online‑only placeholders** – files that exist only in the cloud cannot be backed up by tools that operate locally; see [[concepts/online-only-file-handling]].

---

## Typical Hybrid Workflow (Mac context)
1. **Set cloud as the source of truth** and keep its folder hierarchy consistent.
2. **Sync cloud folders locally** on [[entities/macos]] (mark critical folders as “always keep on this device”).
3. Use a **one‑way backup** tool such as [[entities/carbon-copy-cloner]] or [[entities/chronosync]] to copy from the local cloud folder to the external drive without reverse syncing. See [[concepts/one-way-backup]].
4. Enable versioning/archive options (e.g., SafetyNet in CCC) to retain older copies.
5. Schedule the backup (e.g., weekly) and disconnect the drive.

---

## When to Choose One Over the Other
- **Pure cloud** – If you value minimal hardware, need constant remote access, and are comfortable with subscription costs.
- **Pure external drive** – If you have ample local storage, need fast access, and want complete data ownership with no ongoing fees.
- **Hybrid** – Recommended for most users; the cloud offers daily convenience, while the drive provides a reliable offline snapshot.

---

## Related Concepts
- [[concepts/one-way-backup]] – How to perform a read‑only copy from cloud to drive.
- [[concepts/online-only-file-handling]] – Strategies for dealing with placeholders when backing up.

---

## Source
The guidance is derived from the discussion in [[summaries/session-12_2024-06-15]].