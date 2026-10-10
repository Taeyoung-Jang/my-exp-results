---
type: "Concept"
sources: ["summaries/session-05_2025-06-15.md"]
description: "Framework describing iOS and Android location permission tiers and their privacy impact."
---

# Location Permission Models

**Definition**: A set of permission levels that mobile operating systems expose to control how apps can access a device’s location, balancing functionality with user privacy.

---

## Overview
Mobile platforms provide graduated permission options so users can grant just enough location data for an app to work while limiting unnecessary tracking. The model varies slightly between iOS and Android but shares common principles:

1. **Never / Deny** – No location data is shared.
2. **Ask Next Time / When In Use** – Location is only provided when the app is actively being used.
3. **While Using the App** – Similar to “When In Use” but applies to any foreground activity, blocking background access.
4. **Always / Allow All the Time** – Grants continuous location access, even when the app runs in the background.

These tiers map directly to the permission settings discussed in [[summaries/session-05_2025-06-15]].

---

## Platform‐Specific Details

### iOS (Apple)
- Settings path: **Settings → *App* → Location**.
- Options: **Never**, **Ask Next Time**, **While Using**, **Always**.
- **Precise Location** toggle (under the same screen) lets users choose between exact coordinates and an approximate area.
- With **While Using**, background services like widgets, Live Activities, or Background App Refresh cannot retrieve location unless the app also has the **Always** permission.

### Android (Google)
- Settings path: **Settings → Apps → *App* → Permissions → Location**.
- Options: **Deny**, **Allow only while using the app**, **Allow all the time**.
- “Allow only while using” blocks background location; background access requires the explicit **Allow all the time** grant.
- Some OEMs add extra privacy utilities such as permission auto‑reset.

---

## Precise vs. Approximate Location
Both platforms let users downgrade the granularity of location data. Turning off **Precise Location** (iOS) or **Use precise location** (Android) reduces the fidelity of the data shared, limiting privacy exposure while still satisfying many app functions.

---

## Privacy vs. Functionality Trade‑off
Choosing a permission level involves weighing the app’s core needs against potential privacy risks. For instance, maps or weather apps typically need **While Using** (or **Allow only while using**) to function correctly, whereas shopping or gaming apps can often operate safely with **Never**. This balance is captured in the broader [[concepts/privacy_vs_functionality_tradeoff]] concept.

---

## System Location Services (iOS)
Even when all third‑party apps are set to **Never** or **While Using**, iOS system services (e.g., **Significant Locations**, **Location‑Based Alerts**, **Find My**) may still access location for internal features. These services can trigger the location indicator without exposing data to apps. See [[concepts/system_location_services_ios]] for a deeper dive.

---

## Recommendations
1. **Default to Deny** for apps that do not require location.
2. Use **While Using** (iOS) or **Allow only while using the app** (Android) for apps whose core functionality depends on location (maps, navigation, weather).
3. Turn off **Precise Location** when exact coordinates are unnecessary.
4. Regularly audit Android’s **Allow all the time** list and downgrade any non‑essential apps.
5. Disable iOS **Significant Locations** if you wish to limit system‑level tracking while keeping services like **Find My** active.

---

## Related Concepts
- [[concepts/privacy_vs_functionality_tradeoff]]
- [[concepts/system_location_services_ios]]

---

## Entities Mentioned
- [[entities/iphone]]
- [[entities/android]]
- [[entities/apple]]
- [[entities/google]]
- [[entities/find-my]]
- [[entities/location-based-alerts]]
- [[entities/significant-locations]]
