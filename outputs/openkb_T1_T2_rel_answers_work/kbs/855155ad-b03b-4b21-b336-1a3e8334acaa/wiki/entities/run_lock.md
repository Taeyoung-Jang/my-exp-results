---
sources: ["summaries/session-40_2025-10-15.md"]
type: "Other"
description: "A lockfile ensuring only one offline compute run executes at a time."
---

# Run Lock

**Type:** other

**Description:** A lockfile placed in the run directory to guarantee that only a single instance of the overnight compute script runs, preventing concurrent execution and aiding crash‑recovery.

**Key facts from [[summaries/session-40_2025-10-15]]**
- Created as `$RUN/run.lock` before the script starts.
- Contains the PID of the running process.
- A `trap` removes the lock on normal exit or when interrupted (`INT`, `TERM`).
- The script aborts if the lock already exists, signalling a previous run is still active or crashed.

**Role in the workflow**
- Provides crash safety and enables the resume‑friendly design described in [[concepts/offline_compute_workflow]].
- Works together with `status.json` to let the script skip already‑completed stages.

**Related entities**
- Works alongside [[entities/usb_transfer]] which is used after the lock is released to move the bundle of results.

**See also**
- [[concepts/deep_work_environment]] – the broader context of minimizing distractions while managing long runs.