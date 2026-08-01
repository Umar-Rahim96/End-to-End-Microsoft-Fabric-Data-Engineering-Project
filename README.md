# End-to-End Data Engineering Pipeline using Microsoft Fabric

## Overview

This project demonstrates an end-to-end data engineering solution built using Microsoft Fabric. The pipeline automatically ingests CSV files from Azure Data Lake Storage Gen2, transforms the data using PySpark, stores the processed data in a Lakehouse following the Medallion Architecture (Bronze, Silver, and Gold), creates Gold tables in a Fabric Data Warehouse, and uses Power BI for reporting and visualization.

The goal of this project was to gain hands-on experience in designing and implementing a complete data engineering workflow using Microsoft Fabric.

---

## Technologies Used

- Microsoft Fabric
- Azure Data Lake Storage Gen2
- Microsoft Fabric Data Factory
- Lakehouse
- PySpark
- Microsoft Fabric Data Warehouse
- SQL
- Power BI
- Git & GitHub

---

## Project Workflow

### Data Source
The source data consists of CSV files stored in Azure Data Lake Storage Gen2.

### Data Ingestion
A Microsoft Fabric Data Factory pipeline automatically ingests the source files.

The pipeline uses the following activities:

- Get Metadata
- Filter
- ForEach
- If Condition
- Set Variable
- Copy Activity

These activities make the pipeline dynamic and reusable for processing multiple files.

### Bronze Layer
The ingested data is stored in the Bronze layer of the Lakehouse without any transformations. This layer preserves the original raw data.

### Data Transformation
A PySpark notebook performs data transformation by:

- Removing duplicate records
- Handling missing values
- Renaming columns
- Converting data types
- Preparing the data for analytics

### Silver Layer
The transformed data is stored in the Silver layer of the Lakehouse.

### Gold Layer
Business-ready Fact and Dimension tables are created in the Microsoft Fabric Data Warehouse for reporting and analysis.

### Reporting
Power BI connects to the Gold tables through a semantic model to create interactive dashboards.

---

## Repository Contents

This repository contains:

- 📁 **[architecture](./architecture/)** – Project architecture diagram.
- 📁 **[notebooks](./notebooks/)** – PySpark notebook used for data transformation.
- 📁 **[pipeline](./pipeline/)** – Documentation related to the Microsoft Fabric Data Factory pipeline.
- 📁 **[powerbi](./powerbi/)** – Power BI report (.pbix).
- 📁 **[sample-data](./sample-data/)** – Sample datasets used in the project.
- 📁 **[screenshots](./screenshots/)** – Screenshots of the pipeline, Lakehouse, Data Warehouse, and Power BI report.
- 📁 **[sql](./sql/)** – SQL scripts used to create tables and views.

---

## Project Files

- Architecture Diagram: `architecture/DataEngineeringworkflow.jpg`
- PySpark Notebook: `notebooks/BronzeToSilverTransformation.ipynb`
- Power BI Report: `powerbi/SalesDashboard.pbix`

---

## Key Features

- Automated data ingestion from Azure Data Lake Storage Gen2
- Dynamic Microsoft Fabric Data Factory pipeline
- Metadata-driven workflow
- PySpark-based data transformation
- Bronze, Silver, and Gold architecture
- Gold tables in Microsoft Fabric Data Warehouse
- Interactive Power BI dashboard

---

## What I Learned

This project helped me gain practical experience in:

- Building automated ETL pipelines using Microsoft Fabric
- Working with Azure Data Lake Storage Gen2
- Developing reusable Data Factory pipelines
- Transforming data using PySpark
- Implementing the Medallion Architecture
- Designing Gold tables in a Data Warehouse
- Creating Power BI reports using curated data

---

## Future Improvements

In the future, this project can be enhanced by adding:

- Incremental data loading
- Pipeline scheduling
- Data quality validation
- Error handling and logging
- CI/CD integration using GitHub

---

## Author

**Umar Rahim**

Computer Science Student | Aspiring Data Engineer

GitHub: https://github.com/yourusername

LinkedIn: https://linkedin.com/in/yourprofile
