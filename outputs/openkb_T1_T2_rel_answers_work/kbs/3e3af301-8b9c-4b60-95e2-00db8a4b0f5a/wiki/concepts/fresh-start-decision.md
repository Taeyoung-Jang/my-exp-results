---
type: "Concept"
sources: ["summaries/session-37_2024-12-01.md"]
description: "Guidelines for deciding when a system reset or reinstall is warranted."
---

# Fresh Start Decision Criteria

## Definition
A set of practical signals that indicate it is more efficient to perform a full system reset or OS reinstall rather than continue incremental troubleshooting.

## Core Signals (from [[summaries/session-37_2024-12-01]])
- **Performance mismatch** – The computer feels slow in ways that do not match its hardware specifications.
- **Recurring instability** – Crashes, glitches, or error loops persist even after standard fixes.
- **Unclear root cause** – Troubleshooting becomes guesswork because the underlying issue cannot be isolated.
- **Software bloat** – Years of fragmented applications, outdated drivers, and background services have accumulated.
- **Time cost** – The effort spent fighting the machine outweighs the time required for a clean reinstall.

## Decision Flow
1. **Assess symptoms** using the core signals above.
2. **Estimate effort**: compare time spent on ad‑hoc fixes vs. time to create a fresh environment.
3. **Check data safety**: ensure a comprehensive [[concepts/backup-checklist]] is in place before proceeding.
4. **Plan migration**: follow [[concepts/data-migration-safety]] to move only essential items.
5. **Track licenses**: verify all product keys and activation files via [[concepts/license-tracking]] before wiping.
6. **Execute** the reset/reinstall on the target platform (e.g., [[entities/windows]] or [[entities/macos]]).

## Relationship to Other Concepts
- This criteria is a subset of the broader [[concepts/fresh-start-decision]] framework.
- It relies on a solid [[concepts/backup-checklist]] to avoid data loss.
- Safe migration of needed items is covered by [[concepts/data-migration-safety]].
- Proper handling of software keys and activation files is addressed by [[concepts/license-tracking]].

## Practical Example
A user on both [[entities/windows]] and [[entities/macos]] notices frequent freezes and cannot pinpoint the cause after multiple driver updates and app removals. The performance slowdown is disproportionate to the hardware, and troubleshooting has consumed several days. Applying the Fresh Start Decision Criteria, the user decides a clean OS reinstall is the most efficient path, first completing the backup checklist, then migrating only SSH keys, email archives, and essential license files.
