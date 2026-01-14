# Lab 2.4 — Repository Setup

This repository is the setup for Lab 2.4. It contains the Week 1 restaurant CSV files and a Databricks notebook that will be used to practice reproducible ETL and logging.

## Folder structure

- `data/`
  Stores the input CSV files used by the notebook:
  - `menu_items.csv`
  - `order_details.csv`

- `logs/`
  Stores log files created by the notebook when it runs.

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
