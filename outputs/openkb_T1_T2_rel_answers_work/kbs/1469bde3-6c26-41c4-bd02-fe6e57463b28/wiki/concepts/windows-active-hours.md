---
type: "Concept"
sources: ["summaries/session-38_2025-02-15.md"]
description: "Time window that blocks automatic Windows updates and restarts during active use."
---

## Windows Active Hours

**Definition**: *Windows Active Hours* is a user‑defined time range during which Windows Update will not automatically install updates or trigger a forced restart. The feature lets users keep their device stable while they are actively working, and defer any disruptive changes to off‑hours.

**Key Details from [[summaries/session-38_2025-02-15]]**
- Set via **Settings → Windows Update → Active hours**.
- Can be fixed (e.g., 09:00 – 17:00) or let Windows infer usage patterns and adjust automatically.
- Works on both Windows 11 Pro and Home; on Home the setting is the primary tool for avoiding surprise changes because true feature‑update deferral is unavailable.
- When active hours are in effect, Windows will postpone installation of non‑security updates, optional/preview updates, and system reboots until the defined window closes.

**Configuration Steps (Windows 11 Home)**
1. Open **Settings** → **Windows Update**.
2. Click **Change active hours**.
3. Choose **Manually set active hours** and enter your work‑day start and end times, or select **Automatically adjust active hours** to let Windows learn your usage.
4. Confirm the selection.

**Interaction with Other Update Controls**
- **Pause updates** can be layered on top of active hours for short crunch periods (up to 1 week).
- The **Get the latest updates as soon as they’re available** toggle (found in *Advanced options*) further reduces the chance of surprise feature rolls‑out; if missing, active hours combined with manual avoidance of the *Download and install* button is the fallback.
- Disabling **Microsoft Store auto‑updates** (via *Microsoft Store → Profile → App Settings*) prevents app‑level changes inside the active window.

**Relation to Other Concepts**
- Part of a broader [[concepts/software-update-strategy]] that balances stability with security.
- Complements [[concepts/ios-automatic-updates]] on iOS, where a similar “schedule‑only” approach is used.
- Helps mitigate [[concepts/beta-testing-risk-management]] concerns by limiting exposure to preview or beta updates during critical work periods.

**Benefits**
- Predictable workstation behavior during weekdays.
- Allows a dedicated **weekend update routine** (restart, install all pending patches, then reboot) without interrupting productivity.
- Reduces the cognitive load of unexpected restarts or UI changes.

**Limitations**
- Does not prevent all background activity (e.g., security patches may still download, though installation is delayed).
- On some builds, the *Get the latest updates…* toggle may be hidden, requiring manual vigilance.

**See Also**
- [[entities/microsoft]]
- [[entities/windows-11]]
- [[entities/windows-update]]
- [[entities/microsoft-store]]
