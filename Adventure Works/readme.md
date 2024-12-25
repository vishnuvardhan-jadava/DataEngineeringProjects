# Adventure Works Data Engineering Project

## Project Overview
This project demonstrates a complete data engineering pipeline using the Adventure Works dataset available on Kaggle. The pipeline includes data extraction, transformation, and analytics using Azure services and Power BI. The workflow involves:

1. Extracting data from a GitHub repository using Azure Data Factory.
2. Storing raw data in Azure Data Lake (Bronze layer).
3. Transforming the data in Azure Databricks and saving it in the Silver layer.
4. Further refining and loading data into the Gold layer.
5. Building interactive dashboards in Power BI for analytics and visualization.

## Dataset
**Name**: Adventure Works Territories

**Source**: [Adventure Works Dataset on Kaggle](https://www.kaggle.com/datasets/ukveteran/adventure-works?resource=download&select=AdventureWorks_Territories.csv)

The dataset provides information about sales territories, including geographic regions and related sales data.

## Architecture

### Tools and Technologies
- **Azure Data Factory**: Orchestrates data movement and scheduling.
- **Azure Data Lake Storage**: Stores raw, transformed, and refined data.
- **Azure Databricks**: Processes and transforms the data.
- **Power BI**: Visualizes insights and trends.

### Pipeline Stages

1. **Extract (Bronze Layer)**
   - Data is downloaded from the GitHub repository hosting the Adventure Works dataset.
   - Azure Data Factory pipelines automate the extraction process and store the raw data in Azure Data Lake.

2. **Transform (Silver Layer)**
   - Azure Databricks processes the raw data to remove inconsistencies and normalize formats.
   - Cleaned data is stored in the Silver layer of Azure Data Lake.

3. **Load (Gold Layer)**
   - Data is further refined and aggregated for analytics.
   - Azure Databricks loads the processed data into the Gold layer.

4. **Analytics and Visualization**
   - Power BI connects to the Gold layer for real-time analytics and interactive dashboards.

## Steps to Reproduce

### Prerequisites
1. Azure Subscription with:
   - Azure Data Factory
   - Azure Data Lake Storage
   - Azure Databricks
2. Power BI Desktop installed locally.
3. GitHub account to host the dataset.

### Workflow

1. **Setup GitHub Repository**
   - Clone the dataset from Kaggle.
   - Upload the dataset to a GitHub repository.

2. **Azure Data Factory**
   - Create a pipeline to extract the dataset from the GitHub repository.
   - Configure a linked service to connect to Azure Data Lake Storage.
   - Store the raw data in the Bronze layer.

3. **Azure Databricks**
   - Create a Databricks workspace.
   - Develop notebooks to clean and transform the raw data into Silver and Gold layers.
   - Save transformed data back to Azure Data Lake.

4. **Power BI**
   - Connect Power BI to the Gold layer in Azure Data Lake.
   - Build dashboards to visualize key metrics such as sales trends and geographic performance.

## Deliverables
- **Bronze Layer**: Raw dataset stored in Azure Data Lake.
- **Silver Layer**: Cleaned and normalized dataset.
- **Gold Layer**: Aggregated and analytics-ready dataset.
- **Power BI Dashboards**: Interactive visualizations of sales performance.

## Results
The pipeline enables:
- Seamless integration of GitHub-hosted datasets with Azure services.
- Scalable and efficient data transformation.
- Comprehensive analytics using Power BI.

## Future Enhancements
- Incorporate additional datasets to enrich analytics.
- Automate Power BI report generation using Power BI Service.
- Implement real-time data processing with Azure Stream Analytics.

## Repository Structure
