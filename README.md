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

See `RUN.md` for the exact steps to run the notebook in Databricks.
