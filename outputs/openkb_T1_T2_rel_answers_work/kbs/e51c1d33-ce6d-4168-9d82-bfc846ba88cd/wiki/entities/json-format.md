---
sources: ["summaries/session-38_2024-12-13.md"]
type: "Product"
description: "JSON is a lightweight data-interchange format used for storing structured data in the study plan."
---

## JSON (product)

JSON (JavaScript Object Notation) is a text‑based, language‑independent format for representing structured data. In the **7‑hour weekly study plan** described in [[summaries/session-38_2024-12-13]], JSON is recommended for the file‑based project because it handles hierarchical records such as habit entries or bookmarks more naturally than flat tables.

### Why JSON was chosen
- Supports nested objects, making it ideal for storing items with multiple attributes (e.g., habit name, date, status) as shown in the sample schema.
- Allows easy reading and writing in Python using the built‑in `json` module, aligning with the suggested project skeleton.
- Contrasted with [[entities/csv-format]], which is better for simple, uniform rows, JSON was deemed the smoother option for the tracker project.

### Related concepts and workflow
- The decision process is part of the broader **[[concepts/weekly-study-plan]]** that balances practice, API work, and file‑based projects.
- The project follows the **[[concepts/api-project-workflow]]** pattern for the Open‑Meteo API task, while the JSON project mirrors the same incremental milestone approach.
- Logging progress follows the **[[concepts/learning-log-template]]**, ensuring reflections on JSON usage are captured.

### Practical usage in the study plan
- **File‑based project**: A habit tracker or bookmark manager stores its data in a `habits.json` (or similar) file.
- **Python helpers**: Functions like `load_data()` and `save_data()` use `json.load` and `json.dump` to persist the data.
- **Extensibility**: The JSON file can later be expanded with additional fields without changing the overall storage format.

---

*Entity reference: [[entities/json-format]]*