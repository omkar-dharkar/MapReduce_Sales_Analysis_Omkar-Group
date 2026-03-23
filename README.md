# Liquor Sales Analysis using Hadoop MapReduce

A big data analytics project focused on processing and analyzing large-scale liquor sales data using **AWS RDS**, **Apache HBase**, **Apache Sqoop**, and **Hadoop MapReduce**.

This project was completed as part of a **Big Data** assignment. I served as the **team lead of a 4-member group**, managing the project flow, coordinating task execution, and guiding the end-to-end implementation from data ingestion to analytical reporting.

---

## Project Objective

The goal of this project was to gain hands-on experience in processing large datasets and generating business insights using modern big data tools and cloud-based systems.

The project was designed to strengthen practical understanding of:

- Data ingestion using cloud platforms such as AWS RDS
- Data movement from relational databases to NoSQL systems using Apache Sqoop
- Data storage design in Apache HBase
- Data cleaning and preparation for reliable analysis
- Batch processing using Hadoop MapReduce
- Business analytics and insight generation from large transactional datasets

This project bridges the gap between theoretical big data concepts and real-world data analytics implementation.

---

## Business Context

The liquor industry is a major contributor to the retail economy, especially in regions where alcohol sales are regulated and transaction data is closely tracked. Analyzing liquor sales helps businesses understand customer demand, regional performance, vendor contribution, and product popularity.

Using sales records from **2020 to 2025**, this project aimed to uncover patterns that can support:

- inventory optimization
- category-level sales planning
- county-level market analysis
- store performance benchmarking
- vendor evaluation
- time-based sales trend analysis

The final output of the project includes data-driven recommendations to improve business operations and profitability.

---

## Dataset Overview

The dataset contains detailed liquor sales records across multiple stores and counties, including transactional, geographic, vendor, product, and financial attributes.

### Key fields in the dataset

- Invoice / Item Number
- Date
- Store Number
- Store Name
- Address
- City
- Zip Code
- Store Location
- County Number
- County
- Category
- Category Name
- Vendor Number
- Vendor Name
- Item Number
- Item Description
- Pack
- Bottle Volume (ml)
- State Bottle Cost
- State Bottle Retail
- Bottles Sold
- Sale Dollars
- Volume Sold (Litres)
- Volume Sold (Gallons)

These attributes enabled both operational analysis and business-focused reporting.

---

## Project Tasks

### 1. Data Ingestion and Preparation

The first stage involved loading and structuring the liquor sales dataset for distributed analysis.

#### Tasks performed
- Uploaded the dataset into **AWS RDS** with appropriate schema design
- Structured tables according to the dataset dictionary
- Split and prepared data where required for efficient ingestion
- Transferred data from **AWS RDS to HBase** using **Apache Sqoop**
- Designed HBase schema with suitable row keys and column families
- Validated the ingested data across systems for consistency and completeness

---

### 2. Data Cleaning

Before analysis, the dataset was cleaned to improve reliability and accuracy.

#### Cleaning steps
- Removed rows with missing or incomplete values
- Handled inconsistent formatting and invalid records
- Standardized relevant categorical and textual fields
- Corrected structural issues in the data where needed
- Eliminated duplicate records to maintain integrity

---

### 3. Batch Processing using Hadoop MapReduce

MapReduce jobs were used to process the dataset and answer business analytics questions at scale.

#### Revenue and Sales Analysis
- Calculated **total revenue per store**
- Identified **top-selling liquor categories**
- Aggregated county-level metrics including:
  - total sale dollars
  - total volume sold in litres
  - total volume sold in gallons

#### Store and Vendor Performance
- Ranked stores based on:
  - total revenue
  - total volume sold
  - average sales per transaction
- Ranked vendors using:
  - total sale dollars
  - total sales volume

#### Time-Based Trend Analysis
- Analyzed liquor sales trends over time
- Studied monthly and yearly revenue patterns
- Evaluated volume-based sales trends using transaction dates

---

## Key Deliverables

This repository includes the major outputs and supporting files created during the project, such as:

- Jupyter notebook implementation
- execution logs
- result tables
- analytical summaries
- supporting report files
- business recommendations

Depending on the version of the repository, the files may include:
- cleaned output datasets
- store performance summaries
- vendor performance reports
- county-level revenue analysis
- category sales trends
- MapReduce execution logs
- project report or PDF documentation

---

## Tech Stack

- **AWS RDS**
- **Apache HBase**
- **Apache Sqoop**
- **Hadoop MapReduce**
- **Python / Jupyter Notebook**
- **Excel**
- **PDF reports and execution logs**

---

## Repository Structure

A typical structure of this repository is as follows:

```text
Liquor_Sales_Analysis_MapReduce/
│
├── Hadoop_and_MapReduce_Assignment_*.ipynb
├── MRJOBs_Execution_Log.pdf
├── Liquor Sales Analysis Solution Instruction.pdf
├── county_level_sales.xlsx
├── liquor_sales_trends.xlsx
├── store_performance.xlsx
├── top_selling_categories.xlsx
├── total_revenue_by_store.xlsx
├── vendor_performance.xlsx
└── README.md
