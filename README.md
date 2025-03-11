# Project-Azure-Data-Engineering-Pipeline
This project automates data ingestion from Kaggle to GitHub, processes it using Azure Data Factory, Databricks, and Synapse, and visualizes insights in Power BI, showcasing an end-to-end data pipeline.

Goal: Automate the process of pulling datasets from Kaggle to GitHub, ingesting them into Azure Data Lake using Azure Data Factory (ADF), processing them in Databricks, storing them in another storage container, and visualizing insights in Power BI via Synapse.

### Step 1: Extract Data from Kaggle to GitHub
Tools: Kaggle API, GitHub Actions
Use Kaggle API to download the dataset programmatically.
Push the dataset to a GitHub repository.
Automate this using GitHub Actions (or a simple Python script run on a schedule).

### Step 2: Ingest Data from GitHub to Azure Data Lake
Tools: Azure Data Factory (ADF), Azure Data Lake Storage (ADLS)
Use ADF Pipelines to dynamically pull data from GitHub.
Store raw data in Azure Data Lake Storage Gen2 (ADLS).

### Step 3: Process & Transform Data using Databricks
Tools: Azure Databricks, PySpark
Load data from ADLS into Azure Databricks.
Perform data cleansing, transformations, and aggregations.
Write the processed data back to a separate storage container in ADLS.

### Step 4: Load Data into Azure Synapse Analytics
Tools: Azure Synapse Analytics, PolyBase
Use Synapse Pipelines or Direct Query to load transformed data from ADLS into Synapse Dedicated SQL Pool.
Optimize table structures for analytical queries.

### Step 5: Visualize in Power BI
Tools: Power BI, Azure Synapse (Direct Query)
Connect Power BI to Azure Synapse for visualization.
Create dashboards and reports based on the transformed data.
