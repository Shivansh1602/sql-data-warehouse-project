# sql-data-warehouse-project

SQL Data Warehouse — End-to-End ETL Pipeline
A complete, production-style data warehouse built from scratch using Microsoft SQL Server, implementing Medallion Architecture and Star Schema dimensional modelling for scalable, analytics-ready data infrastructure.

Project Overview
This project demonstrates an end-to-end ETL (Extract, Transform, Load) pipeline that ingests raw business data from two source systems — ERP and CRM — and transforms it into a structured, query-optimised data warehouse. The pipeline follows the industry-standard Medallion Architecture, progressing data through three distinct layers: Bronze (raw ingestion), Silver (cleansing and transformation), and Gold (analytical reporting).

The final Gold layer exposes a Star Schema model — with a central fact table surrounded by dimension tables — designed for fast, intuitive BI queries and reporting.

Architecture
The warehouse is structured around three medallion layers:

Bronze Layer — Raw CSV data is ingested as-is into SQL Server using BULK INSERT. No transformations are applied; this layer preserves full source history.

Silver Layer — Data is cleaned and standardised: duplicates removed, nulls handled, data types enforced, and business rules applied.

Gold Layer — Analytics-ready Star Schema built here, consisting of fact_sales, dim_customers, and dim_products, connected via surrogate keys.

Tech Stack
Database: Microsoft SQL Server 2022 (via Docker on Mac)

Query Language: T-SQL

IDE: VS Code with MSSQL extension

Containerisation: Docker Desktop (linux/amd64 emulation on ARM64)

Version Control: Git & GitHub

Diagramming: Draw.io

Key Concepts
ETL pipeline design, Medallion Architecture, Star Schema & dimensional modelling, surrogate vs. natural keys, data cleansing, stored procedures, data quality validation, and end-to-end documentation.

