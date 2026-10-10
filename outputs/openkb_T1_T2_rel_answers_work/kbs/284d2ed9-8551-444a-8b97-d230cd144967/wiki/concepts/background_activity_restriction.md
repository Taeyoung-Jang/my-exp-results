---
type: "Concept"
sources: ["summaries/session-36_2025-01-14.md", "summaries/session-07_2024-07-14.md"]
description: "Limiting apps from running in the background to reduce tracking and battery use."
---

# Background Activity Restriction

**Definition** – A privacy‑ and battery‑saving measure that stops apps from executing code when they are not actively in use. By restricting background activity, a device reduces the amount of data an app can collect while the user is unaware.

## Implementation on Android
- Open **Settings → Apps → [App] → Battery**.
- Choose **Restricted** (or *Background restriction* on some versions).
- Optionally also disable **Background data** under *Mobile data* for the same app.
- This prevents the app from running in the background unless you open it, which cuts down on silent location, sensor, or network use.

## Implementation on iPhone (iOS)
- The closest equivalent is turning off **Background App Refresh** for individual apps in *Settings → General → Background App Refresh*.
- While not named the same, the goal is identical: stop apps from updating when they are not in the foreground.

## Why it matters for privacy
- Many apps collect location, device identifiers, or usage metrics continuously. Restricting background activity limits these hidden data flows.
- Reduced background execution also conserves battery and data, providing a tangible benefit beyond privacy.

## Relationship to other privacy concepts
- Works hand‑in‑hand with [[concepts/location_permissions]]: when an app cannot run in the background, occasional location checks are less likely to occur.
- Complements [[concepts/ad_personalization]] by cutting off background data that can feed ad‑network profiling.

## Platform references
- The Android approach is described in the context of [[entities/android]].
- The iOS approach references the iPhone environment (see [[entities/iphone]] and [[entities/apple]] for broader system settings).

## Source
These guidelines are drawn from the privacy checklist in [[summaries/session-07_2024-07-14]].

See also: [[summaries/session-36_2025-01-14]]