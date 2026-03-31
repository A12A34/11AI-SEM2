# Codex Instructions - 11AI-SEM2

## Project Overview

This repository contains school work for Year 11 Semester 2.

The project currently has two main areas:

- `school/ML` for machine learning notebooks and datasets
- `school/WEB` for web lessons and HTML/CSS/JavaScript tasks

## Repository Structure

```text
school/
  ML/
    code/
    data/
  WEB/
    lessons/
    tasks/
```

### ML Area

- Notebooks are the main deliverables.
- Keep executable ML work in `school/ML/code/`.
- Keep datasets in `school/ML/data/`.

### WEB Area

- Lessons live in `school/WEB/lessons/`.
- Practice assignments live in `school/WEB/tasks/`.
- Each task folder may contain a standalone HTML file, assets, and an activity document.

## Working Conventions

These conventions are based on `.github/copilot-instructions.md` and the current repo layout.

### For Machine Learning Work

- Prefer Jupyter notebooks over standalone Python scripts.
- Use relative paths only.
- From notebooks in `school/ML/code/`, load datasets with paths like `../data/<filename>`.
- Do not use absolute paths or Windows backslashes in notebook examples.
- Start every code cell with a short `#` comment explaining the cell.
- Use `pandas` as `pd`.
- Show DataFrames by leaving the variable as the last line in the cell instead of using `print()`.
- Prefer `pd.concat()` over deprecated `df.append()`.

### For Web Tasks

- Keep files simple and beginner-friendly.
- Favor plain HTML, CSS, and JavaScript unless the task clearly requires a library.
- Use relative asset paths such as `images/Apple.png`.
- When fixing JavaScript behavior, make the smallest clear change first.
- Prefer readable variable names and straightforward DOM logic.

## Current Known Context

### Machine Learning

- Notebook found: `school/ML/code/data_wrangiling.ipynb`
- Dataset found: `school/ML/data/Titanic-Dataset.csv`

### Web

- Lessons exist under `school/WEB/lessons/lesson-1`, `lesson-2`, and `lesson-3`
- A standalone lesson file also exists: `school/WEB/lessons/memory-card.html`
- Tasks currently exist under `school/WEB/tasks/task1` through `task7`

### Current Active Task

- File: `school/WEB/tasks/task7/Fruit-Game.html`
- Related assets are in `school/WEB/tasks/task7/images/`
- The game uses image swapping and win/loss counters
- The stop logic was fixed by storing the interval ID and clearing that stored timer

## Preferred Codex Behavior

- Read nearby files before changing code.
- Preserve the current folder structure.
- Keep solutions appropriate for a school project.
- Do not over-engineer simple exercises.
- When editing notebook-related guidance, stay aligned with the Copilot instructions.
- When editing web tasks, prioritize clarity and correctness over abstraction.

## Common Paths

- ML notebook folder: `school/ML/code`
- ML data folder: `school/ML/data`
- WEB lessons folder: `school/WEB/lessons`
- WEB tasks folder: `school/WEB/tasks`
- Current task file: `school/WEB/tasks/task7/Fruit-Game.html`

## Notes For Future Updates

- Expand this file if the repo gains more subjects under `school/`.
- Add run or preview instructions if a consistent workflow is introduced.
- Keep this file synced with `.github/copilot-instructions.md` when that file changes.
- Add a section for `school/AI` if that subject is introduced.
- Add a section for `school/GameDev` if that subject is introduced.
- Add a section for `school/Robotics` if that subject is introduced.
