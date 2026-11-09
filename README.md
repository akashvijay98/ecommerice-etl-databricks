# E-Commerce Analytics ETL Pipeline

## Overview

An end-to-end data engineering project built with Databricks, PySpark, SQL, and Delta Lake to transform raw e-commerce datasets into analytics-ready tables.

## Architecture

The pipeline follows the Medallion Architecture:

- **Bronze:** Ingests raw customer, order, product, order-item, and payment datasets into Delta tables.
- **Silver:** Performs data cleansing, type conversion, validation, and deduplication.
- **Gold:** Builds curated datasets for daily sales, product performance, and geographic revenue analysis.

## Technology Stack

- Databricks
- PySpark
- Spark SQL
- Delta Lake
- Unity Catalog

## Dataset

Five e-commerce CSV files containing customer, order, product, order-item, and payment information.

## Pipeline Workflow

1. Upload CSV files to a Unity Catalog volume.
2. Ingest raw datasets into Bronze Delta tables.
3. Apply cleansing and validation transformations in Silver.
4. Generate analytical reporting tables in Gold.
5. Query curated tables using Databricks SQL.

## Results

The pipeline produces analytical tables supporting revenue analysis, product performance reporting, and country-level sales insights.

## Project Screenshots

Add screenshots of the Databricks tables, pipeline job execution, and dashboard.

## Running the Pipeline

Import the notebooks into a Databricks workspace, configure the Unity Catalog paths, upload the source datasets, and execute the notebooks in Bronze → Silver → Gold order.
