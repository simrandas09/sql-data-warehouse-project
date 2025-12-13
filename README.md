# SQL Data Warehouse and Analytics Project

This repository showcases an end‑to‑end **data warehousing and analytics solution** built with SQL Server. It demonstrates the complete lifecycle from ingesting raw CSV data, designing a modern data warehouse, implementing ETL pipelines, and developing analytical SQL queries for business insights.

## 🔍 Project Summary

- Designed and built a **modern data warehouse** in SQL Server using a **Medallion Architecture**:
  - **Bronze layer** for raw ERP and CRM CSV ingestion.
  - **Silver layer** for data cleansing, standardization, and integration.
  - **Gold layer** for business-ready **star schema** optimized for analytics.
- Developed **ETL pipelines** to:
  - Load raw CSV files into staging (Bronze) tables.
  - Apply data quality rules (duplicate removal, null handling, type casting, standardization).
  - Transform and integrate ERP + CRM data into a unified sales model.
- Implemented **analytics and reporting** queries focused on:
  - Customer behavior and segmentation.
  - Product and category performance.
  - Sales trends and key KPIs.

## 🧱 Tech Stack

- **Database**: SQL Server / SQL Server Express  
- **Development & Querying**: SQL, SQL Server Management Studio (SSMS)  
- **Version Control**: Git & GitHub  
- **Design & Documentation**: draw.io (architecture & data model diagrams), Notion (project planning & phases)

## 🏗️ Data Architecture

The warehouse follows a **Bronze–Silver–Gold Medallion** pattern:

- **Bronze (Raw Layer)**  
  - Ingests ERP and CRM CSV files into SQL Server with minimal transformation.  
  - Preserves the original structure for traceability and auditing.

- **Silver (Cleansed & Integrated Layer)**  
  - Standardizes data types, formats, and reference keys.  
  - Cleanses data (handling nulls, duplicates, invalid values).  
  - Integrates ERP and CRM data into consolidated tables.

- **Gold (Business Layer / Star Schema)**  
  - Contains **fact and dimension tables** designed for analytics, including:
    - Fact: Sales / Orders
    - Dimensions: Customer, Product, Date, Geography (and others as needed)
  - Optimized for BI tools and performant analytical querying.

## 🧠 Data Modeling

- Designed a **star schema** to support common sales analytics scenarios.  
- Defined primary/foreign keys, surrogate keys, and appropriate indexes.  
- Ensured conformed dimensions to enable consistent reporting across multiple subject areas.

## 📊 Analytics & Reporting

Prepared SQL-based analytics to answer key business questions:

- **Customer Behavior**
  - Top customers by revenue and order volume.
  - New vs. returning customers.
  - Basic customer lifetime value style metrics (where data allows).

- **Product Performance**
  - Best-selling products and categories.
  - Revenue contribution per product line/segment.
  - Identification of underperforming products.

- **Sales Trends**
  - Monthly and quarterly revenue trends.
  - Regional and channel performance.
  - Seasonality and growth patterns over time.

These queries can be used directly or connected to BI tools such as Power BI or Tableau for dashboarding.

## 📂 Datasets

- Source data provided as **CSV files** representing:
  - ERP data (orders, order lines, products, etc.)
  - CRM data (customers and related attributes)  
- CSVs are loaded into the **Bronze layer**, then transformed through **Silver** into the **Gold** star schema.

## 🎯 Learning & Portfolio Goals

This project is part of my **data engineering / analytics portfolio** and demonstrates:

- SQL development for ETL and analytics  
- Data warehouse design using Medallion Architecture  
- Star schema data modeling  
- Practical experience with data quality, integration, and performance‑oriented SQL
