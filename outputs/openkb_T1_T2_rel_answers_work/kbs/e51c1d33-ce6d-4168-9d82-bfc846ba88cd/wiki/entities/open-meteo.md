---
sources: ["summaries/session-38_2024-12-13.md"]
type: "Product"
description: "Free weather and geocoding API service for developers."
---

# Open-Meteo (product)

Open-Meteo is a free, public weather API that provides current and forecast data without requiring authentication. It also offers a geocoding endpoint that converts city names to latitude/longitude coordinates, simplifying location‑based queries.

## Key facts from [[summaries/session-38_2024-12-13]]
- Used as the core of a **3‑hour API project** in a 7‑hour weekly study plan for Python learners.
- The project pipeline follows the [[concepts/api-project-workflow]]: geocode → fetch weather → parse → CLI display.
- Calls are made with the Python [[entities/requests]] library and the responses are handled as JSON, leveraging the [[entities/json-format]] data format.
- The API requires no API key, making it ideal for quick prototyping and learning exercises.

## Related concepts & entities
- [[concepts/weekly-study-plan]] – the broader learning schedule that incorporates the Open-Meteo project.
- [[entities/requests]] – the HTTP client used to query the service.
- [[entities/json-format]] – the format of the weather data returned by Open-Meteo.

---
*Page generated for internal knowledge base.*