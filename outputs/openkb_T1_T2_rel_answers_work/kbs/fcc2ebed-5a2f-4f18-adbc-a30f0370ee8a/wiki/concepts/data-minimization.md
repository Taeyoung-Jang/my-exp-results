---
type: "Concept"
sources: ["summaries/session-32_2025-09-12.md"]
description: "Limiting stored data to the minimum needed for recovery and functionality."
---

# Data Minimization

**Definition**: Data minimization is the practice of collecting, storing, and retaining only the amount of personal or device data that is strictly necessary to achieve a specific purpose, such as backup and recovery.

## Why It Matters for Mobile Cloud Backups

In the context of mobile devices, excessive backup data increases exposure risk, consumes cloud storage, and may enable unwanted profiling. The session‑32 discussion highlights several privacy and security concerns that are mitigated by applying data‑minimization principles:

- Reducing the attack surface if the cloud account is compromised.
- Lowering the impact of a provider breach.
- Limiting the amount of personal information that can be used for personalization or ads.

## Key Practices (derived from [[summaries/session-32_2025-09-12]])

1. **Audit Backup Categories** – Review which data types are included in the backup (e.g., app data, call history, location history, voice recordings) and disable any non‑essential categories.
2. **Separate Media Sync** – Keep photo and contact sync enabled (through services like [[entities/google-photos]] or [[entities/icloud]]) while turning off their inclusion in full device backups.
3. **Selective App Backups** – On iPhone, use the iCloud Storage list to toggle off large or sensitive apps; on Android, adjust Google Backup settings per app.
4. **Limit Analytics & Logs** – Disable detailed usage logs or device analytics that are not required for restoration.

## Relationship to Other Concepts

- **[[concepts/backup-reliability]]** – While reliable backups are essential, data minimization ensures that reliability does not come at the cost of unnecessary data exposure.
- **[[concepts/end-to-end-encryption]]** – Encrypting the minimal set of data you retain provides stronger protection, as there is less plaintext for an attacker to target.
- **[[concepts/risk-assessment]]** – Data minimization is a core component of any risk‑assessment strategy, lowering both likelihood and impact of data‑related incidents.

## Practical Checklist

- Enable end‑to‑end encryption for the remaining backup data. end to‑end‑encryption
- Turn on two‑factor authentication on cloud accounts.
- Review and prune the list of devices and third‑party apps with access.
- Disable backup of non‑essential app data, call logs, and analytics.
- Keep only essential items (device settings, photos, contacts) in the backup.

By following these steps, users achieve a balance between **recoverability** and **privacy**, adhering to the principle of data minimization.
