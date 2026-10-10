---
sources: ["summaries/session-05_2025-06-15.md"]
type: "Other"
description: "iOS feature that logs frequent places to improve system services."
---

# Significant Locations

Significant Locations is an iOS system service that records the places you visit most often. The data is used by Apple to power features such as time‑sensitive suggestions, route optimization, and other location‑based system improvements.

## Privacy considerations
- The service can cause the location arrow to appear even when no third‑party app has location permission.
- It does **not** share location data with apps that are set to "While Using" or "Never".
- Turning it off reduces system‑level tracking while preserving useful functions like Find My.

## Relevant concepts and entities
- Related concept: [[concepts/system_location_services_ios]] – describes how iOS system services use location.
- Related concept: [[concepts/privacy_vs_functionality_tradeoff]] – the balance between useful system features and privacy.
- Related concept: [[concepts/location_permission_models]] – outlines the permission levels for apps.
- Associated Apple devices: [[entities/iphone]], [[entities/apple]].
- Connected services: [[entities/find-my]], [[entities/location-based-alerts]].
- Android counterpart discussion: [[entities/android]], [[entities/google]].

## Source
- This information is drawn from the conversation summary [[summaries/session-05_2025-06-15]].