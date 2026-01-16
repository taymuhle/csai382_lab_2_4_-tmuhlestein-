# Lab 2.4 — GitHub Repository Setup (Reproducible ETL)

This repository is the required project structure for Lab 2.4. It is designed to support reproducible ETL work in Databricks using sample restaurant order data.

## Folder purposes

- `notebooks/`
  Contains Databricks notebooks for this project.
  - Main notebook: `lab_2_4_repro_logging`

- `sql/`
  Reserved for SQL scripts (transformations/queries) used by the pipeline.

- `etl_pipeline/`
  Reserved for Python modules or scripts that implement the ETL pipeline outside of notebooks.

- `data_samples/`
  Contains the input sample datasets used for the lab:
  - `menu_items.csv`
  - `order_details.csv`

## How to run

Updated upstream
See `RUN.md` for the exact steps to run the notebook in Databricks.

## Files

- `README.md`
  Project overview and folder descriptions.

- `RUN.md`
  Exact steps to reproduce a run in Databricks.

## How to run in Databricks

1. In Databricks Workspace, open this repo as a Git folder.
2. Open the notebook `lab_2_4_repro_logging`.
3. Run all cells from top to bottom.
4. Verify that the notebook reads the CSVs from `data/` and writes logs into `logs/`.

Some info just shouldn't end up in logs. For example, anything that can identify a person (names, emails, addresses, etc.) is a bad idea because logs get copied around and stored forever, and that can turn into a privacy mess fast. Also, never log secrets like API keys, access tokens, or passwords, since leaking those can basically hand someone the keys to your systems. Reproducibility helps with accountability because you can rerun the same pipeline and prove how you got a result instead of guessing. It also helps with fairness because it makes it easier to audit changes and confirm differences in outcomes come from real updates, not random noise or a slightly different environment.
Stashed changes
