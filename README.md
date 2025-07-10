#  Olympic Data Analytics | Azure End-To-End Data Engineering Project

##  Project Overview

This project showcases an **End-to-End Data Engineering Pipeline** built using **Microsoft Azure services**. We process and analyze Olympic data using tools like **Azure Data Factory**, **Data Lake Gen2**, **Azure Synapse Analytics**, and **Azure Databricks**.

The focus is on understanding how to build a modern cloud-based data pipeline, from raw data ingestion to final analytics and reporting.

---

##  Technologies Used

- **Azure Data Factory (ADF)** – For data ingestion and orchestration
- **Azure Data Lake Storage Gen2** – As the cloud data lake for storing raw and processed data
- **Azure Synapse Analytics** – For data warehousing and analytics using SQL
- **Azure Databricks** – For data transformation and advanced processing (PySpark)
- **Power BI / Synapse Studio** – For data visualization and exploration (optional)

---

##  Dataset

The Olympic dataset includes information about:
- Athlete performance
- Countries and regions
- Medal counts
- Event details

You can use publicly available datasets such as from:
 [Olympics Dataset on Kaggle](https://www.kaggle.com/datasets/the-guardian/olympic-games)

---

##  Project Workflow

1. **Data Ingestion using ADF**
   - Copy Olympic data from local or web source to Azure Data Lake Storage Gen2 (raw zone).

2. **Data Storage**
   - Store data in **Data Lake Gen2** with structured folder hierarchy: `raw`, `processed`, `curated`.

3. **Data Transformation using Azure Databricks**
   - Read raw data from the lake.
   - Perform cleaning, joining, and transformation using **PySpark**.
   - Write the cleaned data to the `processed` zone in the lake.

4. **Data Loading into Synapse Analytics**
   - Load processed data from the lake into **Azure Synapse SQL tables**.
   - Use **Synapse Pipelines or ADF** for this step.

5. **Data Analysis using Synapse / Power BI**
   - Run analytical queries using T-SQL in Synapse.
   - Optional: Create dashboards in Power BI using Synapse as the source.

---

##  Key Concepts Covered

- Building a cloud-native data pipeline on Azure
- Ingesting, transforming, and analyzing structured data
- Using PySpark in Databricks for data engineering tasks
- Querying big data in Synapse with serverless SQL
- Orchestrating data flow using Azure Data Factory

---

##  Notes

- Ensure proper IAM roles are assigned to allow services to access the Data Lake.
- Databricks cluster must have access to your storage account and Synapse endpoint.
- Keep your data zone structure consistent: raw → processed → curated.

