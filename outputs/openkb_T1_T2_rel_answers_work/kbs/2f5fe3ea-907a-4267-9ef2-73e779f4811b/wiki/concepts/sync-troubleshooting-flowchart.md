---
type: "Concept"
sources: ["summaries/session-37_2025-02-15.md", "summaries/session-14_2024-06-15.md"]
description: "A step‑by‑step flowchart‑style checklist for efficiently diagnosing sync issues."
---

# Sync Troubleshooting Flowchart

## Definition
A concise, flowchart‑style procedure that guides users through the quickest checks to isolate and resolve cross‑device sync problems without performing a full reset.

## Origin
This flowchart originates from the conversation in **[[summaries/session-14_2024-06-15]]**, where the assistant distilled a troubleshooting order into a clear "if‑yes/no then" checklist.

## Step‑by‑Step Checklist
1. **Account Sign‑In** – Verify the same account is logged in on all devices.  
   - *If wrong, correct the login and re‑test sync.*
2. **Network Connectivity** – Ensure both devices have a stable internet connection.  
   - *If flaky or offline, reconnect before proceeding.*
3. **App Responsiveness** – Confirm the sync‑related app/service is open and not frozen.  
   - *If frozen, force‑quit and relaunch.*
4. **Power / Battery Mode** – Check that devices are not in low‑power or battery‑saving mode that may throttle background activity.  
   - *If enabled, disable it and retry sync.*
5. **OS & App Versions** – Make sure the operating system and relevant apps are up‑to‑date.  
   - *If outdated, install updates then re‑test.*
6. **Background & Data Permissions** – Verify the app is allowed to run in the background and use mobile data.  
   - *If restricted, adjust permissions.*
7. **Storage Availability** – Check local device storage and cloud account quota.  
   - *If near full, free space before continuing.*
8. **Final Soft Reset** – Relaunch the app on all devices; if still failing, reboot the devices.  
   - *If issues persist, consider a temporary server‑side outage.*

## How to Use
- Follow the checklist from top to bottom; each step includes a quick "yes/no" decision point.
- The early steps are designed as **one‑minute checks** to save time.
- Only move to the next step after confirming the current one is not the root cause.

## Related Concepts
- [[concepts/cross-device-syncing]] – The broader context in which reliable sync is essential.
- [[concepts/sync-feature-prioritization]] – Highlights which sync features are most critical, informing which parts of the flowchart may need extra attention (e.g., messaging sync).

---
*Page last updated based on the source summary of session‑14 (2024‑06‑15).*

See also: [[summaries/session-37_2025-02-15]]