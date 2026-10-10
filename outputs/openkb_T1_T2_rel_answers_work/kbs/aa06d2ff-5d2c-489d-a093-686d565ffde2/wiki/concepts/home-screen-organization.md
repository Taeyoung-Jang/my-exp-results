---
type: "Concept"
sources: ["summaries/session-39_2024-12-13.md"]
description: "Techniques for arranging apps and managed icons on mobile device home screens."
---

# Home Screen Organization

**Definition**: The practice of structuring app icons, folders, and pages on a mobile device’s home screen to balance personal use and corporate management constraints.

---

## Overview
Home screen organization becomes critical when a device is under [[concepts/mobile-device-management]] (MDM) or [[concepts/supervised-mode]]. Users must keep personal apps easily reachable while complying with policies that place restricted, gray placeholder icons on the home screen.

The guidance in [[summaries/session-39_2024-12-13]] outlines a practical workflow for both iOS and Android devices, focusing on moving managed icons into a single folder (or a dedicated last page) and ensuring the personal page remains the default view.

---

## iOS (iPhone) Workflow
1. **Enter edit mode** – Long‑press any app icon until the icons wobble.
2. **Create a folder** – Drag a restricted (gray) icon onto another restricted icon to form a folder, or use an existing folder.
3. **Collect all managed icons** – Drag every supervised icon into the folder.
4. **Move the folder to the far‑right** – While still in edit mode, drag the folder to the edge of the screen until it flips to the next page, repeating until it lands on the last home‑screen page.
5. **Set personal page as primary** – iOS always treats the left‑most page as the default home screen, so keep personal apps on that page.
6. **Handling new apps** – New managed apps will appear on the first available page; users must manually drag them into the work folder or last page.

> **Note**: There is no iOS setting to stop new managed apps from auto‑appearing; the App Library does not block them from visible pages.

---

## Android Workflow
- **With a Work Profile**: Managed apps appear in a separate work‑profile section marked with a briefcase badge. Personal apps stay on the main screen, eliminating clutter.
- **Without a Work Profile**: Apply the same folder‑or‑last‑page technique as iOS. Users can also use a custom launcher (if not blocked by MDM) to hide or reorder icons.

---

## Supporting Strategies
- **Staging Folder** – Using a dedicated folder (see [[concepts/staging-folder]]) acts as a “catch‑all” for managed apps, simplifying future clean‑up.
- **Collaboration with IT** – Ask the [[entities/it-department]] if a work/personal profile split can be enabled; this is often the cleanest long‑term solution.

---

## Related Concepts
- [[concepts/mobile-device-management]] – Governs how devices are supervised.
- [[concepts/supervised-mode]] – Describes device‑wide restrictions that affect icon manipulation.
- [[concepts/staging-folder]] – A folder used to temporarily hold items before final placement.

---

## Entities Mentioned
- [[entities/ios]]
- [[entities/iphone]]
- [[entities/android]]
- [[entities/it-department]]
- [[entities/smartphone]]

---

## References
- Session summary: [[summaries/session-39_2024-12-13]]
