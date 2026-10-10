---
type: "Concept"
sources: ["summaries/session-36_2025-01-14.md", "summaries/session-07_2024-07-14.md"]
description: "Guidance on configuring app location permissions to balance utility, privacy, and battery life."
---

# Location Permissions

## Overview
Location permissions determine how apps can access your device’s location data. By adjusting these settings you can protect privacy, conserve battery, and keep essential services—such as maps, rideshare, and weather—usable.

## Permission Modes
- **Precise vs. Approximate**: Precise location reveals exact coordinates; approximate location shares only a coarse area. Use approximate by default and switch to precise only when actively navigating. This follows the recommendations in [[concepts/precise_vs_approximate_location]].
- **While Using vs. Always**: "While using the app" grants access only when the app is in the foreground. "Always" allows background tracking and should be avoided for most apps unless continuous location is essential (e.g., turn‑by‑turn navigation, fitness tracking, geofencing). See [[concepts/location_privacy_tradeoff]] for the broader trade‑off discussion.
- **Background Refresh**: Disabling background refresh prevents apps from continuously collecting location data when not in use. Pair this with limiting "Always" permissions to reduce background activity.
- **Geofencing**: Where possible prefer geofencing over constant background tracking; apps can trigger actions only when you enter or leave defined areas, offering comparable convenience with less data collection. [[concepts/geofencing]]

## Recommended Settings per App
| App Type | Permission | Precision | Background Refresh |
|----------|------------|-----------|--------------------|
| Maps (e.g., Apple Maps, Google Maps) | **While using** | Approximate by default; enable precise only during active navigation | Off unless you need real‑time traffic alerts |
| Rideshare (Uber, Lyft) | **While using** | Precise only during an active ride/pickup | Off |
| Weather | **While using** or **Never** (set city manually) | Approximate is sufficient | Off |
| Fitness / Safety (e.g., running trackers) | **Always** (if continuous tracking is required) | Precise for accurate activity mapping | Keep background refresh on only for these trusted apps |
| Smart‑home / Automation | **Always** (for geofencing) | Approximate is usually enough | Off |

## Platform‑Specific Guidance
- **iPhone**: Adjust permissions via **Settings → Privacy & Security → Location Services**. For each app set the mode to *While Using* and turn **Precise Location** off unless the app needs exact coordinates. Disable **Significant Locations** in *System Services* to stop the device from building a detailed movement history. Limit **Background App Refresh** to the few apps that truly need it. [[concepts/ios_location_settings]]
- **Android**: Open **Settings → Apps → [App] → Permissions** and choose *While using the app*, selecting approximate where possible. Use **Battery** settings to set apps to *Restricted* for background activity. Consider turning off unnecessary system location services that feed ad‑personalization.

## Checklist for Auditing Permissions (plain text)
1. Review each app’s location mode; downgrade from *Always* to *While Using* wherever feasible.
2. Switch to *Approximate* location unless precise data is essential.
3. Disable **Background App Refresh** for apps that do not require real‑time updates.
4. Monitor battery usage screens for apps that consume disproportionate power – a red flag for hidden background location.
5. Observe the location‑service icon; if it lights up when no app is in the foreground, investigate the responsible app.

## Related Concepts
- [[concepts/ad_personalization]] – Reducing tracking through ad settings.
- [[concepts/background_activity_restriction]] – Limiting apps’ background activity to complement location controls.

## Source
This guidance is derived from the discussions in [[summaries/session-07_2024-07-14]] and the updated recommendations from [[summaries/session-36_2025-01-14]].