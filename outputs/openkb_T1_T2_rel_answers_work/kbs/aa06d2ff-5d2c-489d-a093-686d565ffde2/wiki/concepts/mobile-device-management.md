---
type: "Concept"
sources: ["summaries/session-39_2024-12-13.md"]
description: "MDM is a system that enforces policies on mobile devices like iOS and Android."
---

# Mobile Device Management

**Definition**: Mobile Device Management (MDM) is a set of technologies and policies used by organizations to control, secure, and monitor smartphones and tablets deployed to employees.

## Core Functions
- Enroll devices into a management server.
- Apply configuration profiles that restrict settings, install or block apps, and enforce security policies.
- Remote actions such as wipe, lock, or push updates.
- Monitor compliance and generate reports for the [[entities/it-department]].

## Interaction with Home‑Screen Organization
MDM can place **restricted placeholder icons** on the home screen of managed devices. Users can often **re‑arrange** these icons into folders or move them to a later page, but cannot delete them without violating policy. This ties directly into the concept of [[concepts/home-screen-organization]], where users manage visible layout while staying within MDM constraints.

## Supervised vs. Managed Modes on iOS
On iOS, MDM may operate in two modes:
- **Supervised mode** – full device control; users cannot delete managed icons, only move them. See [[concepts/supervised-mode]].
- **Managed‑apps‑only mode** – lighter control; users may have more flexibility to hide or uninstall managed apps.

The distinction can be checked via **Settings → General → VPN & Device Management**.

## Android Work Profile
When MDM uses an Android **Work Profile**, managed apps appear in a separate section marked with a briefcase badge. This isolates work‑related icons from personal ones, reducing clutter on the personal home screen.

## Practical Tips from [[summaries/session-39_2024-12-13]]
- **Folder method**: Drag all managed gray icons into a single folder and move the folder to the last home‑screen page.
- **Page method**: Individually drag each managed icon to the rightmost page.
- **No auto‑hide**: iOS provides no setting to automatically prevent new managed apps from appearing on the primary page; users must manually move them.
- **App Library**: Helpful for personal apps but does not block supervised apps from showing on active pages.

## Benefits
- Centralized security and compliance.
- Ability to enforce corporate policies on personal devices (BYOD).
- Remote management capabilities for lost or compromised devices.

## Challenges
- User experience can be impacted by visible managed placeholders.
- Limited ability for users to customize the home screen without violating policy.
- Need for clear communication between users and the [[entities/it-department]] to balance security with usability.

---
*Related concepts*: [[concepts/home-screen-organization]], [[concepts/supervised-mode]]
