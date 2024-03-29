# london-fire-incident-data-engineering-analysis
# Fire Incident Data Pipeline

## Overview

This GitHub repository contains the code and configuration files for a data pipeline that ingests, processes, and analyzes fire incident data. The pipeline is implemented using various Azure services such as Azure Data Factory, Azure Data Lake, and Azure Databricks.

![data architecture](https://drive.google.com/uc?export=view&id=1bnooflAagd6zdeL8aP59rddHcqxE5dEG)

## Key Components

### 1. Data Ingestion

- The fire incident data is ingested from an HTTP source link using Azure Data Factory.
- The ingestion process is facilitated by the Copy Data Activity within Azure Data Factory.
- 
![azure data factory](https://drive.google.com/uc?export=view&id=1o24fKw_0pHQUEIz5BZy00-DMZgmqycCO)

### 2. Storage

- The ingested data is stored in Azure Data Lake for efficient and scalable data storage.

### 3. Data Processing

- PySpark is used within Azure Databricks for processing the stored fire incident data.
- The preprocessing logic is implemented using PySpark for data transformation and enrichment.

### 4. Intermediate Storage

- The preprocessed data is stored back in Azure Data Lake, serving as an intermediate storage layer.

### 5. Analysis
The power Bi file : [download](https://drive.google.com/file/d/1NR1mmNl2RP1a5aR70uDWYJGjPBDofbks/view?usp=drive_link)

![data modle](https://drive.google.com/uc?export=view&id=1kYwcFfu614BkA3FsKLAkYR1RwsTD-4Kk)

![page1](https://drive.google.com/uc?export=view&id=1zfd7lvLWCq2s2iTg2ZnxgevYOS_l1ubB)
![page 2](https://drive.google.com/uc?export=view&id=1-Bj3zsbdRhIY0xShRgodEM_yqRfvwBF8)
![page 3](https://drive.google.com/uc?export=view&id=15eMu1qsQZX6UvdyBPLugEbG-gl4px0oJ)
![page 4](https://drive.google.com/uc?export=view&id=1ogMXbhLB0BSEgXoE8yxra1CkiN6D1o6_)


- Power BI is utilized for analyzing the preprocessed fire incident data stored in Azure Data Lake.
- Power BI reports and dashboards can be created to derive insights and visualize trends in the data.

## Setup and Configuration

To set up and configure the pipeline, follow these steps:

1. Clone the repository to your local machine.
2. Configure the Azure Data Factory pipeline with the appropriate HTTP source link for fire incident data.
3. Ensure Azure Data Lake is set up and accessible for storing the ingested and preprocessed data.
4. Configure Azure Databricks with the necessary PySpark scripts for data processing.
5. Update Power BI connections to point to the Azure Data Lake storage for analysis.

## Usage

Once the pipeline is set up and configured, you can execute it to ingest, process, and analyze fire incident data seamlessly. Monitor the pipeline execution for any issues and review Power BI reports for insights.

Feel free to customize the pipeline according to your specific requirements or enhance it further to accommodate additional data sources or analysis techniques.

## Contributing

If you find any issues or have suggestions for improvements, please open an issue or submit a pull request. Contributions are welcome!
