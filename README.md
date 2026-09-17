# 🚀 Data Warehouse & Analytics Project



Welcome to the **Data Warehouse and Analytics Project** repository! This project demonstrates an end-to-end data warehousing and analytics solution—from building an enterprise data warehouse using SQL Server to modeling data and generating actionable business insights.

Designed as a production-grade portfolio project, it highlights industry best practices in data engineering, ETL pipeline construction, and analytical reporting.

---

## 🏗️ Data Architecture

This project implements the **Medallion Architecture**, organizing data into three distinct layers to ensure quality, traceability, and performance:


```

[ ERP / CRM CSV Sources ]
│
▼
📜 BRONZE LAYER   ──►  Raw Data Ingestion (SQL Server)
│
▼
🧹 SILVER LAYER   ──►  Cleansing, Standardization & Normalization
│
▼
⭐ GOLD LAYER     ──►  Business-Ready Star Schema (Facts & Dimensions)

```

1. **🥉 Bronze Layer**: Stores raw data as-is from source systems. Data is ingested directly from CSV files into SQL Server staging tables.
2. **🥈 Silver Layer**: Applies data cleansing, transformation, deduplication, and standardization rules to prepare data for analytical modeling.
3. **🥇 Gold Layer**: Houses business-ready data modeled into an optimized **Star Schema** designed for high-performance reporting and analytics.

---

## 📖 Project Overview

This repository showcases the complete data engineering and analysis lifecycle:

* **Data Architecture**: Designing a Modern Data Warehouse utilizing Medallion Architecture.
* **ETL Pipelines**: Extracting, transforming, and loading data across Bronze, Silver, and Gold layers using SQL Server.
* **Data Modeling**: Developing dimensional models (Fact and Dimension tables) optimized for BI queries.
* **Analytics & Reporting**: Writing SQL-based analytical queries to deliver actionable business metrics.

### Key Skills Demonstrated
- SQL Development & Query Optimization
- Data Engineering & Pipeline Design
- Data Architecture & Medallion Framework
- Dimensional Data Modeling (Star Schema)
- Data Quality & Cleansing Frameworks
- Data Analytics & Business Intelligence

---

## 🎯 Project Requirements

### 1. Data Engineering (Building the Warehouse)
* **Objective**: Develop a modern data warehouse in SQL Server to consolidate sales data and enable scalable reporting.
* **Data Sources**: Ingest raw CRM and ERP data supplied via CSV datasets.
* **Data Quality**: Cleanse, resolve missing values, and handle anomalies prior to Gold layer ingestion.
* **Integration**: Unify disparate CRM and ERP records into a single, cohesive data model.
* **Scope**: Target state analytics on current data (historization/SCD is out of scope).
* **Documentation**: Full data dictionary and architectural lineaging provided in `/docs`.

### 2. Data Analysis (BI & Reporting)
* **Objective**: Develop SQL analytics scripts to deliver detailed visibility across key business domains:
  * 👤 **Customer Behavior**: Segmentation, buying patterns, and repeat engagement.
  * 📦 **Product Performance**: Revenue drivers, category performance, and item velocity.
  * 📈 **Sales Trends**: Time-series performance, sales growth, and revenue tracking.



---

## 📂 Repository Structure

```text
data-warehouse-project/
│
├── 📁 datasets/                   # Raw ERP and CRM source files (CSV format)
│
├── 📁 docs/                       # Project documentation & visual architecture
│   ├── etl.drawio                 # ETL pipeline design & processing logic
│   ├── data_architecture.drawio   # Medallion architecture diagram
│   ├── data_flow.drawio           # End-to-end data flow visualization
│   ├── data_models.drawio         # Star Schema ERD diagrams
│   ├── data_catalog.md            # Data dictionary, column definitions & metadata
│   └── naming-conventions.md      # Engineering standards for SQL objects & scripts
│
├── 📁 scripts/                    # Core SQL transformation scripts
│   ├── 📁 bronze/                 # DDL & ingestion procedures for raw data
│   ├── 📁 silver/                 # Data cleansing & transformation scripts
│   └── 📁 gold/                   # Dimension & Fact table creation scripts
│
├── 📁 tests/                      # Data quality & test validation scripts
│
├── 📄 .gitignore                  # Git exclusions
├── 📄 LICENSE                     # Project license
├── 📄 README.md                    # Project landing page
└── 📄 requirements.txt            # Dependencies and tools

```

---

## 🛠️ Getting Started

### Prerequisites

* **Database Engine**: Microsoft SQL Server (2019+ recommended)
* **GUI Client**: SQL Server Management Studio (SSMS) or Azure Data Studio
* **Diagramming**: [Draw.io](https://app.diagrams.net/) (for viewing architecture files in `/docs`)

### Quick Setup

1. **Clone the Repository**:
```bash
git clone (https://github.com/AKRAM339867/sql_data_warehouse_project)
cd data-warehouse-project

```


2. **Execute Ingestion & Transformations**:
* Run scripts in `scripts/bronze/` to create staging tables and load CSV data.
* Run scripts in `scripts/silver/` to execute data cleansing routines.
* Run scripts in `scripts/gold/` to construct the Star Schema analytics views/tables.


3. **Verify Data Quality**:
* Execute verification tests located in `tests/` to confirm data integrity across all layers.



---

## 📜 License

Distributed under the MIT License. See `LICENSE` for more information.


## 👤 About the Author
Hi, I'm Akram Bechat! 👋

I specialize in Finance and Data Analytics, combining business domain knowledge with hands-on data engineering skills (SQL, Python, Excel, Power BI). I enjoy building scalable data pipelines, data warehouses, and reporting systems that transform raw business data into strategic insights.

💼 LinkedIn: [linkedin.com/in/akram-bechat-169651317]

🐙 GitHub: github.com/AKRAM339867

📧 Email: bechat.akram.encg@uhp.ac.ma
```

```
