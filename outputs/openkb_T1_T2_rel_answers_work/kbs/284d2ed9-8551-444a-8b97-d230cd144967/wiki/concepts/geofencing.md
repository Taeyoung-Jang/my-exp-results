---
type: "Concept"
sources: ["summaries/session-36_2025-01-14.md"]
description: "Using geofencing to trigger actions on entry/exit, reducing continuous location tracking."
---

# Geofencing for Privacy‑Friendly Tracking

Geofencing is a location‑based technique that triggers actions when a device **enters** or **exits** a predefined geographic boundary. Instead of continuously streaming GPS coordinates, an app can request location only at these boundary events, markedly reducing the amount of data collected about a user’s movements.

## Why it improves privacy

- **Minimized data collection** – Only the fact that a user crossed a fence is logged, not the precise path taken. This aligns with the [[concepts/location_privacy_tradeoff]] of reducing exposure while retaining functionality.
- **Lower battery impact** – The device’s GPS can stay idle most of the time, similar to the goals of [[concepts/background_activity_restriction]].
- **Fits with approximate location** – Many geofence‑based services work with coarse location, avoiding the need for [[concepts/precise_vs_approximate_location]] “precise” mode.

## Practical use cases mentioned in [[summaries/session-36_2025-01-14]]

- Automation of smart‑home actions (e.g., turning on lights when arriving home).
- Triggering commute‑related updates only when the user leaves or arrives at a work zone.
- Providing “near‑me” recommendations that rely on knowing the user is within a city‑wide area rather than their exact coordinates.

## Implementation tips for iPhone users

1. In **Settings → Privacy & Security → Location Services**, grant the app *While Using* permission and keep **Precise Location** off unless the app explicitly needs it for navigation.
2. Enable the app’s geofence feature; iOS will handle the background checks efficiently.
3. Keep **Background App Refresh** enabled only for the few apps that use geofencing, limiting unnecessary background activity.

## Relation to other concepts

- Works together with [[concepts/location_permissions]] to choose the least‑privileged access level.
- Complements [[concepts/precise_vs_approximate_location]] by allowing coarse location for most checks.
- Serves as an alternative to constant background tracking discussed in [[concepts/background_activity_restriction]].

By adopting geofencing, users can retain convenient, automated location‑based services while substantially lowering privacy risks and battery consumption.