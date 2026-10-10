---
sources: ["summaries/session-32_2024-12-13.md"]
type: "Product"
description: "FreeFileSync is a flexible file‑synchronization utility for Windows and other platforms."
---

# FreeFileSync (product)

FreeFileSync is a free, open‑source **file synchronization** tool that lets users mirror folders across devices. It supports Windows, macOS, and Linux, offering a graphical interface for configuring one‑way or two‑way sync jobs, filter rules, and scheduling.

## Key facts from [[summaries/session-32_2024-12-13]]
- The assistant mentioned FreeFileSync as an alternative to Windows **File History** for mirroring a photo archive to an external drive.
- It provides more granular control than File History but typically requires a manual launch or a scheduled task to run automatically.
- In the discussed workflow, FreeFileSync was noted as less suitable for a completely "plug‑and‑forget" backup approach because of the extra setup steps.

## Related concepts
- [[concepts/plug-and-forget-backup]] – the desired low‑maintenance backup style that File History fulfills more directly.
- [[concepts/external-drive-mirroring]] – the overall goal of keeping a copy of the photo archive on an external drive.
- [[concepts/duplicate-removal]] – a task that can be automated within FreeFileSync using filter rules.

## Related entities
- [[entities/windows]] – the operating system where the discussed setup is applied.
- [[entities/file-history]] – the Windows feature recommended for automatic, plug‑and‑forget backup.

## Comparison with other tools
FreeFileSync offers richer options for selective syncing and conflict resolution compared to the built‑in **File History** feature on [[entities/windows]]. However, achieving a truly automatic sync requires setting up a scheduled task or using third‑party automation, which adds complexity relative to the simplicity of File History.

## Typical use case for travel photo workflow
1. Define a sync job that mirrors the **Photos Archive** folder on the laptop to a folder on the external drive.
2. Optionally configure filters to ignore temporary files or already‑deleted junk.
3. Run the job manually after each trip, or schedule it to trigger when the external drive is connected.

Overall, FreeFileSync is a powerful but slightly more hands‑on solution for users who need fine‑grained control over their backup process.