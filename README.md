# Olympics-Data-Analysis

## Project Overview

The project involved setting up a data processing pipeline using Azure Data Lake Storage Gen2, Azure Data Factory, and Databricks to streamline data ingestion, transformation, and analysis. The goal was to enable seamless data extraction from multiple sources, perform necessary transformations, and prepare the data for visualization and analysis.

## Key Steps

1. Data Lake Storage Setup

  - Created a container in Azure Data Lake Storage Gen2, which included two main folders:
      Raw Data: Used to store unprocessed data directly fetched from multiple sources, providing a base repository for all incoming datasets.
      Transformed Data: Dedicated folder for storing data after transformation, optimized and cleaned for analysis and dashboard creation.

2. Azure Data Factory Pipelines:

  - Configured Azure Data Factory (ADF) pipelines to automate data ingestion and movement:
      Connected ADF to Azure Data Lake Storage Gen2, allowing data extraction from various sources, including GitHub.
      Used a Copy Data activity to load data from these sources into the designated storage account, maintaining a structured and automated data pipeline.

3. Databricks Workspace Setup:

  - Established a Databricks workspace linked to the Azure ecosystem to facilitate scalable data processing and analysis.
  - Configured the workspace to redirect Databricks for streamlined integration with Azure resources.

4. Data Mounting and Analysis:

  - Mounted the raw data stored in Azure Data Lake Storage Gen2 to Databricks for analysis.
  - Completed the app registration process to securely connect Databricks to the data lake, obtaining necessary credentials, including the Client ID, Directory ID, and Secret Key.
  - Assigned Storage Blob Data Contributor access role to ensure Databricks could read/write data efficiently.

5. Data Transformation and Storage:

  - Performed data transformations within Databricks, cleaning and processing the raw data to generate insights and make it ready for dashboard visualization.
  - Stored the transformed data back in the Azure Data Lake Storage Gen2 in the Transformed Data folder, ensuring data is available for downstream applications, including analytics and dashboard tools.

## Outcome

This setup provided a structured and automated data processing workflow, enabling efficient data extraction, transformation, and storage. The transformed data stored in Azure Data Lake is now accessible for visualization, supporting data-driven decision-making through interactive dashboards.
