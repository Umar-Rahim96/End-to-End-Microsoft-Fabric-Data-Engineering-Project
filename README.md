# End-to-End Data Engineering Pipeline using Microsoft Fabric

## Overview

This project demonstrates an end-to-end data engineering pipeline built using Microsoft Fabric. The pipeline ingests CSV files from Azure Data Lake Storage Gen2, performs data transformation using PySpark, stores the processed data in a Lakehouse following the Medallion Architecture, creates Gold tables in a Fabric Data Warehouse, and uses Power BI for reporting.

## Architecture

![Architecture](architecture/Architecture.jpg)

## Technologies

- Microsoft Fabric
- Data Factory
- Azure Data Lake Storage Gen2
- Lakehouse
- PySpark
- Data Warehouse
- SQL
- Power BI
- Git
- GitHub

## Project Workflow

1. CSV files are stored in Azure Data Lake Storage Gen2.
2. A Microsoft Fabric Data Factory pipeline ingests the files.
3. The pipeline uses Get Metadata, Filter, ForEach, If Condition, Set Variable, and Copy Activity to automate processing.
4. Raw data is loaded into the Bronze layer of the Lakehouse.
5. A PySpark notebook cleans and transforms the data.
6. Transformed data is written to the Silver layer.
7. Gold fact and dimension tables are created in the Fabric Data Warehouse.
8. Power BI connects to the semantic model to create reports and dashboards.

## Repository Structure

```
.
├── architecture/
├── notebooks/
├── pipeline/
├── sample-data/
├── screenshots/
├── sql/
└── README.md
```

## Pipeline

![Pipeline](screenshots/Pipeline.jpg)

## Lakehouse

![Lakehouse](screenshots/Lakehouse.jpg)

## PySpark Notebook

![Notebook](screenshots/Notebook.jpg)

## Data Warehouse

![Warehouse](screenshots/Warehouse.jpg)

## Power BI Dashboard

![Dashboard](screenshots/Dashboard.jpg)

## Features

- Automated data ingestion from Azure Data Lake Storage Gen2
- Metadata-driven pipeline
- Reusable ETL workflow
- PySpark data transformation
- Bronze, Silver, and Gold architecture
- Gold tables in Fabric Data Warehouse
- Interactive Power BI reporting

## Skills Demonstrated

- Microsoft Fabric
- Data Engineering
- ETL Pipeline Development
- PySpark
- SQL
- Data Warehousing
- Azure Data Lake Storage Gen2
- Power BI

## Future Enhancements

- Incremental data loading
- Pipeline monitoring
- Data quality validation
- CI/CD with Git integration

## Author

**Umar Rahim**
