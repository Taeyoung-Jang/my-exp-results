---
sources: ["summaries/session-15_2024-06-15.md"]
type: "Other"
description: "RCS is an enhanced messaging protocol offering SMS‑like features with cloud backup."
---

# RCS (Rich Communication Services)

RCS (Rich Communication Services) is a modern messaging protocol that extends traditional SMS with features such as read receipts, typing indicators, high‑resolution photo sharing, and seamless cloud backup. It is the backbone of the chat experience in **Google Messages**, allowing users to enjoy richer communication while still using the carrier’s network.

## Key points from [[summaries/session-15_2024-06-15]]
- In the migration checklist, the assistant emphasizes confirming that **Google Messages** has RCS enabled and that its chat history is included in the system backup.  
- RCS backup is handled via the Android system backup mechanism, which is part of the broader [[concepts/google_backup]] strategy.
- The document notes that RCS is a differentiator when comparing Android and iOS messaging ecosystems (see [[concepts/android_vs_ios]]), as iOS uses iMessage instead.

## Relationships
- Implemented in [[entities/google-messages]] on Android devices.
- Backed up through Google’s cloud backup service managed by [[entities/google]].
- Works alongside other Android communication tools like [[entities/whatsapp]] and [[entities/signal]], though those use their own proprietary protocols.

## Practical considerations
- Ensure RCS is turned on before migrating to a new phone; otherwise, chat history may not be restored.
- RCS data is included in the system‑wide backup, so a recent backup (as instructed in the checklist) will preserve read receipts and media metadata.
- While RCS enhances the Android messaging experience, it does not affect iOS users who rely on iMessage (see [[entities/ios]] and [[entities/apple]]).

---
*This entity page consolidates the information about RCS presented in the session‑15 discussion and links it to relevant concepts and entities within the knowledge base.*