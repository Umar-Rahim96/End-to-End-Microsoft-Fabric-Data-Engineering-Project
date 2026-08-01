# Pipeline Documentation

## Overview

This Microsoft Fabric Data Pipeline automates the ingestion, transformation, and loading of data into the analytics platform.

## Activities

- Copy Activity
- Notebook Activity
- Dataflow Gen2

## Workflow

1. Read source CSV files.
2. Load data into the Bronze Lakehouse.
3. Execute Dataflow Gen2.
4. Run the PySpark notebook.
5. Load transformed data into the Silver Lakehouse.
6. Create Data Warehouse tables.
7. Build the Semantic Model.
8. Create Power BI reports.
