# AWS Python ETL Data Pipeline

## Overview

This project implements a fully automated **ETL (Extract, Transform, Load)** data pipeline using AWS services like S3, Lambda, Glue, and QuickSight. The pipeline processes raw data, performs transformations, and makes it available for visualization and reporting.

### Architecture

The pipeline leverages the following AWS services:

- **Amazon S3**: Stores raw data and transformed data.
- **AWS Lambda**: Automates the process by triggering Glue jobs and other tasks.
- **AWS Glue**: Performs data transformations and data cleaning.
- **AWS Glue Crawlers**: Automatically catalogs data into the Glue Data Catalog.
- **Amazon QuickSight**: Used to visualize the transformed data for business insights.



### Project Goals

- **Data Ingestion**: Extract raw data from a source and load it into S3.
- **Transformation**: Use Glue jobs to transform the raw data into a structured format (Parquet) and perform data cleansing and transformations.
- **Cataloging**: Use Glue Crawlers to automatically catalog the data.
- **Visualization**: Visualize the final transformed data using Amazon QuickSight.

## Key Features

- **Scalable**: Uses serverless technologies (Lambda, Glue) to scale according to data size and processing needs.
- **Automated**: Automatically triggers processes using S3 events and AWS Lambda.
- **Flexible**: Easily extendable to include more transformations and data sources.
- **Cost-Effective**: Takes advantage of AWS's pay-per-use model for Glue, Lambda, and S3.

## Getting Started

### Prerequisites

- **Python 3.x**: Ensure you have Python installed locally.
- **AWS CLI**: Install and configure the AWS CLI for interacting with AWS services.
- **Boto3**: AWS SDK for Python. Install using:
  ```bash
  pip install boto3
