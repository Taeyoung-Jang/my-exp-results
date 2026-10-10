---
sources: ["summaries/session-38_2024-12-13.md"]
type: "Product"
description: "A free public API providing Pokémon data in JSON format."
---

# PokéAPI

**Type:** product  
**Category:** Public web API

## Overview
PokéAPI is an open, unauthenticated web service that delivers extensive data about Pokémon, including species, abilities, moves, and game mechanics. All responses are JSON, making it easy to consume from Python scripts using the `requests` library.

## Key facts from [[summaries/session-38_2024-12-13]]
- Recommended in the 7‑hour weekly study plan as a concrete example for the **API project** slot.
- Suggested project: a small command‑line tool that looks up a Pokémon name and prints its basic stats.
- Integrated into the step‑by‑step workflow described in [[concepts/api-project-workflow]].

## Typical usage pattern
1. **Make a request** – use `requests.get("https://pokeapi.co/api/v2/pokemon/<name>")`.
2. **Parse JSON** – the response follows the [[entities/json-format]] schema.
3. **Display or store** – extract fields such as `base_experience`, `height`, `weight`, and print them or write to a file.

## Relation to other entities
- Works alongside other free APIs like [[entities/open-meteo]] when building multi‑API tools.
- Frequently accessed from Python code, often together with the `[[entities/requests]]` library.
- Data can be saved in either JSON or CSV; for simple tabular exports see [[entities/csv-format]] and [[entities/json-format]].

## Why it’s useful for learners
- No authentication hurdles, allowing focus on **request handling**, **JSON parsing**, and **CLI design**.
- Provides a real‑world dataset to practice data extraction and error handling, fitting neatly into the [[concepts/api-project-workflow]] taught in the study plan.