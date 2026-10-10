---
type: "Concept"
sources: ["summaries/session-40_2025-10-15.md"]
description: "A self‑contained, crash‑safe method for running long jobs on an offline machine."
---

# Offline Compute Workflow

**Definition**: A self‑contained, crash‑safe method for running long jobs on an offline machine.

## Core Elements
1. **Folder layout & naming**
   - Run folder named `YYYY‑MM‑DD_<tag>` (e.g., `2026‑03‑17_mesh‑exp`).
   - Subfolders: `config/`, `code/`, `checkpoints/`, `outputs/`, plus top‑level `run.log`, `status.json`, and a `bundle/` for transfer.
2. **Script responsibilities**
   - Create the run folder and subfolders.
   - Snapshot the current code (git commit hash or full copy) into `code/`.
   - Copy the required config files into `config/`.
   - Execute a series of jobs sequentially, each writing to a unified log and optionally checkpointing.
   - Record completed stages in a JSON status file so the workflow can be resumed after a crash.
   - Prepare a single `bundle/` directory containing the log, outputs, and status for easy USB transfer.
3. **Crash safety & resume support**
   - A lockfile (`run.lock`) prevents concurrent runs.
   - Signal traps clean up the lockfile on exit.
   - `status.json` holds an array of completed stage names; the script skips any stage already listed.
4. **Offline transfer**
   - At morning review, copy only the `bundle/` folder to a USB drive (`[[entities/usb_transfer]]`).
   - The main machine reads the log and status to determine success without re‑opening the offline environment.

## Related Concepts
- [[concepts/deep_work_environment]] – structuring the physical and digital workspace to minimise distractions while using the offline workflow.
- [[concepts/workflow_factors]] – considerations such as reliability, repeatability, and minimal supervision that motivate an offline compute workflow.

## Source Summary
The detailed procedure and script examples are documented in [[summaries/session-40_2025-10-15]].