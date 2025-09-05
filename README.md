# Retail Pricing Analytics

An end-to-end data orchestration solution for analyzing daily vendor pricing across retail outlets. Built using **Azure Data Factory**, **Azure Databricks**, and **Power BI**, this project ingests daily price data via HTTP, transforms it, and delivers actionable insights through interactive dashboards.

---

## Project Overview

Retailers like D-Mart source loose commodities (grains, nuts, vegetables, etc.) from multiple vendors at varying prices. This solution enables:

- Daily ingestion of vendor pricing via HTTP
- Transformation and aggregation using PySpark notebooks
- Visualization of daily prices, monthly averages, and comparisons
- Email alerts on ingestion or transformation failures

---

## Architecture

HTTP Source --> ADF Pipeline: Ingestion (Bronze Layer) --> ADB Notebook: Transformation & Aggregation (Silver and Gold Layers) --> Power BI Dashboard: Modeled using Star Schema

- **ADF**: Orchestrates daily triggers, notebook execution, and refresh logic  
- **ADB**: Performs data cleaning, joins, and time-series aggregation  
- **Power BI**: Displays pricing trends and comparisons

---

## Repo Structure
/adf
/adb
/power_bi

---

## Status

Currently in development (`dev` environment)  
Targeting a production-ready demo with live dashboard and alerting

---

## License

This project is licensed under the MIT License.
