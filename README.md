# Lab 5: Regex, Cleaning, Joins, and Pipelines

In this lab, you will turn imperfect General Conference data into a reproducible, analysis-ready dataset.

## Setup

1. Open a terminal in this repository.
2. Run `uv sync`.
3. Open `lab_5.qmd` in Positron.
4. Complete the code and written-response sections.
5. Render with `uv run quarto render lab_5.qmd`.

## Data

- `data/raw/talks_raw.csv`: talk-level raw data.
- `data/raw/speaker_metadata_raw.csv`: speaker-level metadata with intentional data-quality issues.
- `data/processed/`: destination for the generated cleaned dataset.

Do not manually edit the raw CSV files. Your pipeline should recreate the processed data from code.

## Submission

Follow the submission and GitHub collaborator instructions provided by your instructor.
