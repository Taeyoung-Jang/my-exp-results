---
sources: ["summaries/session-36_2025-01-14.md", "summaries/session-07_2024-07-14.md"]
type: "Product"
description: "Apple iPhone smartphone with detailed privacy and location controls."
---

# iPhone

The iPhone is Apple’s flagship smartphone running iOS. It provides a comprehensive set of privacy controls that let users balance functionality—such as maps, rides‑share, and weather—with minimal data collection.

## Key privacy settings highlighted in [[summaries/session-07_2024-07-14]] and [[summaries/session-36_2025-01-14]]
- **Location permissions** – Use *While Using the App* for most apps and enable *Approximate* location by default, turning on *Precise* only when exact coordinates are required (e.g., navigation). See [[concepts/location_permissions]] and [[concepts/precise_vs_approximate_location]].
- **System location services** – Disable *Significant Locations* under Settings → Privacy & Security → Location Services → System Services to stop Apple from building a detailed movement history. Keep essential services like Find My iPhone enabled. This aligns with the broader trade‑off discussion in [[concepts/location_privacy_tradeoff]].
- **Geofencing support** – Prefer apps that use geofencing instead of constant background tracking for automated routines. The concept is explained in [[concepts/geofencing]].
- **Background activity** – Limit Background App Refresh (Settings → General → Background App Refresh) to only the apps that power your commute or local recommendations, reducing background data collection. Related concept: [[concepts/background_activity_restriction]].
- **Precise vs. Approximate location** – Set *Precise Location* off for apps that only need a rough area (e.g., restaurant recommendations) and keep it on for navigation or safety‑critical apps. See [[concepts/precise_vs_approximate_location]].
- **iOS‑specific toggles** – The collection of settings (Precise Location, Significant Locations, Background App Refresh, and other System Services) is covered under [[concepts/ios_location_settings]].
- **Photo access** – Change app access from *All Photos* to *Selected Photos* via Settings → Privacy & Security → Photos.
- **Ad personalization** – Turn off Apple Advertising in Settings → Privacy & Security → Apple Advertising, matching the recommendation to disable targeted ads in [[concepts/ad_personalization]].
- **App tracking** – Disable *Allow Apps to Request to Track* to block cross‑app tracking.

## Related entities and concepts
- [[entities/apple]] – The manufacturer of the iPhone.
- [[entities/apple_advertising]] – Apple’s advertising platform that can be disabled.
- [[concepts/location_permissions]] – Guidance on configuring location access.
- [[concepts/ios_location_settings]] – Specific iOS toggles for location and background activity.
- [[concepts/background_activity_restriction]] – Android analogue; on iPhone the analogue is limiting background app refresh.
- [[concepts/geofencing]] – Using location triggers without continuous tracking.
- [[concepts/precise_vs_approximate_location]] – Choosing between exact and coarse location data.
- [[concepts/ad_personalization]] – General concept of turning off targeted ads.
