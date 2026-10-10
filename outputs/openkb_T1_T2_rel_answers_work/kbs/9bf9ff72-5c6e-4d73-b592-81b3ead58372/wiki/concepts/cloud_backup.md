---
type: "Concept"
sources: ["summaries/session-33_2024-10-15.md", "summaries/session-08_2024-06-15.md"]
description: "Cloud backup stores files off‑site via the internet, offering automated, versioned protection."
---

# Cloud Backup

**Definition**: Cloud backup is the practice of automatically copying digital files from a local device to an off‑site service accessible over the internet. It provides continuous, versioned protection and can be accessed from anywhere.

## Key Characteristics
- **Automatic syncing** – Files are uploaded in the background without manual intervention.
- **Versioning** – Multiple historic copies are retained, allowing recovery from accidental edits or deletions.
- **Encryption** – Data should be encrypted both in transit and at rest to safeguard privacy.
- **Cost‑effective** – Many providers offer tiered pricing, making it affordable for personal use.

## Role in a Backup Strategy
Cloud backup forms the *online* layer of the classic [[concepts/backup_strategy]] that follows the 3‑2‑1 rule: one primary copy, one off‑site copy, and optionally an offline copy. It is a key component of a [[concepts/low_stress_backup]] because it runs continuously with no user interaction. In the scenario described in [[summaries/session-08_2024-06-15]], the user already employs a reputable cloud service as the automatic layer, complementing an [[concepts/offline_backup]] on an encrypted external drive.

The later discussion in [[summaries/session-33_2024-10-15]] reinforces this role and adds that cloud backup should be paired with an **auto‑run backup software** that starts local backups (including optional full‑disk images) the moment the external drive is connected. This hybrid setup—cloud sync plus a weekly offline backup—embodies the [[concepts/hybrid_backup_approach]] while keeping the overall system low‑stress.

## Best Practices (as illustrated in the source documents)
1. **Choose a reputable provider** that offers versioning and strong encryption.
2. **Enable two‑factor authentication (2FA)** for the cloud account.
3. **Combine with an offline backup** for protection against cloud‑service outages, ransomware, or account lockouts.
4. **Maintain a simple folder hierarchy** to keep the backup organized and consistent.
5. **Verify cloud sync regularly** and run occasional restore checks (e.g., pull a recent file from the cloud and open it) to ensure the backup isn’t silently broken.

## Related Concepts & Entities
- [[concepts/offline_backup]] – The complementary offline storage layer.
- [[concepts/backup_strategy]] – The overall approach that balances convenience, cost, and security.
- [[concepts/low_stress_backup]] – The philosophy of minimizing manual effort.
- [[concepts/hybrid_backup_approach]] – Combining cloud sync with periodic full‑disk or file‑level backups.
- [[entities/time_machine]] – Example of a native macOS tool that can sync to a cloud‑enabled drive.
- [[entities/file_history]] – Windows native tool that works alongside cloud backup for file versioning.

---
*This concept page synthesizes the role and recommendations for cloud backup as presented in the session‑08 and session‑33 discussions.*