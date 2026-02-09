# Copilot Instructions — 11AI-SEM2

## Project Overview

This is a **high-school AI/ML course repository** (Year 11, Semester 2). Work is organized under `school/` by topic, with Jupyter Notebooks for hands-on exercises and accompanying datasets.

## Repository Structure

```
school/
  ML/
    code/    # Jupyter Notebooks (.ipynb) — all executable code lives here
    data/    # Datasets (CSV files) used by notebooks
```

- **Notebooks are the primary deliverable** — not standalone `.py` scripts.
- Datasets sit in `school/ML/data/`; notebooks sit in `school/ML/code/`.

## Conventions

### File Paths
- Always use **relative paths** from the notebook's location.
- From `code/` to `data/`: `../data/<filename>` (e.g., `pd.read_csv("../data/Titanic-Dataset.csv")`).
- Never use absolute or Windows-style backslash paths.

### Notebook Style
- **Every code cell must have a leading `#` comment** explaining what the cell does.
- Use `pandas` as the primary data-manipulation library; import as `pd`.
- Display DataFrames by placing the variable name as the last expression in a cell (no `print()`).
- Prefer `pd.concat()` over deprecated `df.append()` for adding rows.

### Python Environment
- Python 3.13+ with basic type-checking enabled (`python.analysis.typeCheckingMode: "basic"`).
- Key dependency: `pandas`. Install via the notebook kernel, not the terminal.

## When Adding New Topics

1. Create a subfolder under `school/` (e.g., `school/DL/`).
2. Mirror the `code/` + `data/` structure inside it.
3. Keep notebooks focused on one concept each; name them descriptively.
