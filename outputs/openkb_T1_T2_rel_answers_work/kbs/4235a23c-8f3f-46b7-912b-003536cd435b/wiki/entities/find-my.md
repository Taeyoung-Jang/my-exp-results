---
sources: ["summaries/session-05_2025-06-15.md"]
type: "Product"
description: "Apple's Find My product for locating devices and friends."
---

# Find My

**Entity type:** product

Find My is Apple’s built‑in service that lets users locate their iPhone, iPad, Mac, AirPods, and share location with friends and family. It relies on the device’s location hardware but **does not expose** that location data to third‑party apps unless the user explicitly grants permission.

## Key facts from [[summaries/session-05_2025-06-15]]
- Listed as a system service that can cause the location arrow to appear even when no third‑party app has location access.
- Considered generally harmless from a privacy‑to‑apps perspective; it operates within iOS’s own ecosystem.
- Turning off **Significant Locations** reduces system‑level tracking while keeping Find My functional.

## Relationships
- Part of the broader set of [[concepts/system_location_services_ios]] that manage device location on iOS.
- Illustrates the [[concepts/privacy_vs_functionality_tradeoff]]: users keep Find My for device security while limiting other system services that track movement.
- Works alongside other location permission models described in [[concepts/location_permission_models]].

## Related entities
- [[entities/iphone]] – the primary platform for Find My.
- [[entities/apple]] – the company that provides the service.
- [[entities/location-based-alerts]] – another iOS system service that can trigger location indicators.
- [[entities/significant-locations]] – a system service often disabled to reduce background tracking.
