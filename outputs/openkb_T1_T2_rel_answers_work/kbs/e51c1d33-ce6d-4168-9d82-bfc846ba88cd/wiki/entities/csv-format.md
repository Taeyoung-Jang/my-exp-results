---
sources: ["summaries/session-38_2024-12-13.md"]
type: "Product"
description: "CSV is a plain‑text file format for storing tabular data."
---

# CSV (Comma‑Separated Values)

CSV (Comma‑Separated Values) is a simple, human‑readable plain‑text format used to represent tabular data where each line corresponds to a row and fields are separated by commas. It is widely supported by spreadsheet programs, databases, and programming languages.

## Key facts from [[summaries/session-38_2024-12-13]]
- The document recommends CSV for **file‑based projects** when the data fits neatly into rows and columns, such as a lightweight expense logger or a simple spreadsheet‑style record.
- CSV is presented as the simpler alternative to **JSON** when the data structure is flat, making it quick to read/write without hierarchical nesting.
- The choice between CSV and JSON is guided by a rule of thumb: use CSV for uniform tabular records and JSON for more complex, nested data.

## Related concepts and entities
- See the decision guidance in [[concepts/weekly-study-plan]] for how the CSV vs JSON choice fits into a broader study workflow.
- For a more structured data format, compare with [[entities/json-format]].
- The CSV format is mentioned alongside the **file‑based project** in the weekly plan, which helps learners decide the appropriate storage format for their Python exercises.

## Usage tips
- Ensure proper escaping of commas within fields (e.g., by quoting fields).
- Use Python’s built‑in `csv` module for reading and writing to avoid manual parsing errors.
- When sharing CSV files, keep encoding consistent (UTF‑8) to prevent character‑set issues.
