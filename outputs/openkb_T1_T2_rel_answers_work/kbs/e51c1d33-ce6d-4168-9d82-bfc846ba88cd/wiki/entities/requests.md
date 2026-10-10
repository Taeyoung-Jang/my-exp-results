---
sources: ["summaries/session-38_2024-12-13.md"]
type: "Product"
description: "Python HTTP library for making web requests."
---

# Requests library

**Type:** product (Python library)

The **Requests** library is a popular Python package that simplifies making HTTP requests. In the *session-38_2024-12-13* study plan, it is the core tool used to interact with the [[entities/open-meteo]] API and to fetch data for the 3‑hour API project. The code snippets rely on `requests.get` to retrieve JSON payloads, which are then parsed and displayed in a minimal CLI.

### Role in the weekly study plan
- Integrated into the [[concepts/api-project-workflow]] for the Open‑Meteo weather fetcher.
- Supports the learner’s practice of handling network I/O, error handling, and JSON parsing within the [[concepts/weekly-study-plan]].
- Demonstrates a concrete example of applying a third‑party product to a real‑world programming task.

### Related concepts and entities
- Works together with [[entities/python]] to build scripts.
- Returns data in JSON format, often stored using [[entities/json-format]] (or occasionally [[entities/csv-format]] for other projects).
- The workflow illustrated in the session aligns with the [[concepts/learning-log-template]] for tracking progress on API‑based exercises.

### Reference
- See the full summary of the session for context: [[summaries/session-38_2024-12-13]].