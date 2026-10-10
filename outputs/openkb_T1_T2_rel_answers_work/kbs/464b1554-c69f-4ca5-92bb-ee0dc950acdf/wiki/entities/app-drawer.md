---
sources: ["summaries/session-02_2024-06-15.md"]
type: "Other"
description: "A UI component on Android that lists all installed apps for quick access."
---

## App Drawer

The **App Drawer** is the Android system UI that displays a scrollable list of every installed application, providing a central location for app discovery and launch. It functions as the primary overflow area for apps that are not placed on the home screens, supporting the [[concepts/phone-organization]] strategy of keeping daily‑use apps on the home pages while relegating the rest to this drawer.

### Key facts from [[summaries/session-02_2024-06-15]]
- Used as the “overflow drawer” counterpart to the iOS [[entities/app-library]].
- Recommended for a minimalist two‑page home‑screen layout: keep daily essentials on the pages and let the rest sit in the App Drawer.
- Works together with [[entities/settings]] for controlling [[concepts/notification-management]] and [[concepts/battery-optimization]] on a per‑app basis.
- Interacts with [[entities/widgets]] when widgets are placed on the home screens, leaving the drawer solely for app icons.

### Related entities and concepts
- Platform: [[entities/android]] (primary host of the App Drawer) and [[entities/ios]] (uses App Library instead).
- Settings that affect the drawer experience: app visibility options, sorting, and hide/show toggles in [[entities/settings]].
- Optimisation considerations: restricting background activity for apps in the drawer can improve [[concepts/battery-optimization]] and reduce unwanted [[concepts/notification-management]].

### Practical usage tips
1. **Keep the drawer clean** – regularly uninstall or disable apps you no longer need.
2. **Leverage search** – use the built‑in search bar to quickly find rarely‑used apps without scrolling.
3. **Combine with folders** – create a few strategic folders on the home screens and place only the most frequently accessed apps there; everything else stays in the App Drawer.
4. **Adjust permissions** – from [[entities/settings]], limit background refresh and location for apps that reside only in the drawer to conserve battery.
