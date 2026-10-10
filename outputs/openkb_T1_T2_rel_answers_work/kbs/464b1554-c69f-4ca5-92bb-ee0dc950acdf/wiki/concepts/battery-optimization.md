---
type: "Concept"
sources: ["summaries/session-33_2025-02-13.md", "summaries/session-02_2024-06-15.md"]
description: "Techniques to reduce battery drain by managing notifications, background activity, and app layout."
---

## Battery Optimization

Battery optimization is the practice of configuring a smartphone to minimize power consumption while preserving essential functionality. It involves adjusting **notifications**, **background activity**, **location services**, and **widget** usage, as well as organizing apps to reduce unnecessary wake‑ups.

### Key Strategies from [[summaries/session-02_2024-06-15]]

1. **Notification Management**
   - Keep banners and sounds only for time‑critical work/chat apps; use badges‑only or disable for social, shopping, and most finance apps.  
   - Enable *Scheduled Summary* for non‑urgent apps to batch alerts.  
   - Related concept: [[concepts/notification-management]].

2. **Background App Refresh / Activity**
   - **iOS**: Turn off *Background App Refresh* for social, shopping, media, and most utilities; leave it on for messaging, maps, health, email, and active widgets.  
   - **Android**: Use *Battery > Background usage* to set apps to *Optimized* or *Restricted*; keep *Unrestricted* only for messaging, navigation, and health‑tracking apps.

3. **Location Services**
   - Set most apps to **"While Using"**.  
   - Reserve **"Always"** for navigation, rideshare, and weather apps.

4. **Widget Usage**
   - Limit to one medium widget (e.g., Calendar or Weather) per home screen to avoid constant background updates.  
   - Related entity: [[entities/widgets]].

### Platform‑Specific Settings

- **[[entities/ios]] / iPhone**
  - Settings → Notifications → adjust banner, badge, and sound per app.
  - Settings → General → Background App Refresh → toggle per app.
  - Settings → Privacy & Security → Location Services → choose usage mode.
  - Use the **App Library** as an overflow drawer.  
  - Related entity: [[entities/app-library]].

- **[[entities/android]]**
  - Settings → Apps → Notifications → enable/disable channels.
  - Settings → Battery → Background usage / Battery optimization → set per‑app limits.
  - Settings → Location → set mode per app.
  - Use the **App Drawer** for overflow.  
  - Related entity: [[entities/app-drawer]].

### Interaction with Phone Organization

Effective battery optimization works hand‑in‑hand with a tidy **[[concepts/phone-organization]]** layout. By concentrating daily‑use apps on the first home screen and relegating rotating or rarely used apps to folders or the app drawer/library, the system reduces the number of icons it must render and the frequency of background checks.

### Summary

Battery optimization combines selective notification settings, controlled background activity, prudent location permissions, and minimal widget usage, all tailored to the specific controls of [[entities/ios]] and [[entities/android]]. When paired with a disciplined **two‑page home screen** layout, these tweaks noticeably extend battery life and improve overall performance.

See also: [[summaries/session-33_2025-02-13]]