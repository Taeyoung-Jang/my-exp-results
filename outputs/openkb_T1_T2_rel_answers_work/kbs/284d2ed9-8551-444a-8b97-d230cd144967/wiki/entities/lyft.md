---
sources: ["summaries/session-07_2024-07-14.md"]
type: "Organization"
description: "Lyft is a ride‑hailing service and transportation‑network company."
---

# Lyft

Lyft is a major **ride‑sharing organization** that connects passengers with drivers via its mobile app.

## Privacy‑focused permission recommendations (from [[summaries/session-07_2024-07-14]])
- **Location**: Set to **"While Using the App"**. Use **approximate location** by default and enable **precise location** only during an active ride or pickup.
- **Background activity**: Turn **background refresh off** for Lyft to prevent the app from running when not in use. This aligns with the [[concepts/background_activity_restriction]] guidance.
- **General permissions**: Review and limit access to microphone, camera, and contacts unless the app explicitly needs them, following the broader [[concepts/location_permissions]] strategy.

## Related platforms
- **Android**: The background‑activity limitation can be configured via the app’s Battery settings on [[entities/android]].
- **iPhone**: Location and other permissions are managed under Settings → Privacy & Security on [[entities/iphone]].

## Comparable services
- Uber – another major ride‑hailing provider ([[entities/uber]]).

These settings allow Lyft to function for navigation and ride coordination while minimizing unnecessary data collection.
