
# Retail Sales Intelligence Platform | Microsoft Fabric

An end-to-end retail analytics engineering project built with Microsoft Fabric, PySpark, SQL, and Power BI.

## Project Overview

This project demonstrates how retail transaction data can be transformed into reliable, analytics-ready data products using a modern medallion architecture.

The solution will ingest raw retail data, apply data quality and transformation rules, create a dimensional data model, and deliver business insights through Power BI.

**Project status:** In progress

## Business Objectives

- Analyze sales revenue and sales volume trends.
- Identify top-performing products and countries.
- Measure customer purchasing behavior and repeat purchases.
- Analyze invoice cancellations and negative-quantity transactions.
- Build a reusable and validated analytics data model.
- Develop interactive Power BI reports for business decision-making.

## Technology Stack

- Microsoft Fabric Lakehouse
- Fabric Data Factory pipelines
- PySpark and Spark SQL
- Fabric Warehouse and T-SQL
- Power BI and DAX
- Git and GitHub

## Data Source

**Dataset:** Online Retail II  
**Provider:** UCI Machine Learning Repository  
**Source:** https://archive.ics.uci.edu/dataset/502/online+retail+ii

The dataset contains retail transaction records across two periods.

The original source data will be preserved. Data cleaning, transaction classification, and business rules will be documented and implemented reproducibly.

## Planned Architecture

1. **Bronze:** Ingest and preserve raw transaction data.
2. **Silver:** Standardize data types, handle missing values, identify duplicates, and classify transactions.
3. **Gold:** Create fact and dimension tables for analytics.
4. **Semantic Model:** Define relationships and validated DAX measures.
5. **Reporting:** Build interactive Power BI reports and communicate business findings.

## Repository Structure

```text
data/
notebooks/
pipelines/
sql/
powerbi/
docs/
tests/
README.md
```

## Data Quality and Validation

The project will include checks for:

- Missing and invalid values
- Duplicate records
- Invalid quantities and prices
- Transaction classification
- Source-to-target reconciliation
- Referential integrity in the dimensional model

## Business Metrics

Planned metrics include:

- Total Sales Amount
- Units Sold
- Distinct Invoices
- Average Order Value
- Monthly Sales Growth
- Cancellation Rate
- Repeat Customer Rate

Metrics will be finalized after source-data profiling and business-rule validation.

## Project Deliverables

- Reproducible data ingestion and transformation workflows
- Documented data model and architecture
- SQL scripts and data-quality checks
- Power BI report and measures
- Setup instructions and project findings

## Limitations

The source dataset does not provide product costs, so profit cannot be calculated reliably without an additional cost source. Negative quantities and cancellation invoices will be investigated and classified using documented rules rather than automatically treated as product returns.

## License and Attribution

The dataset is provided by the UCI Machine Learning Repository under CC BY 4.0. See the official dataset page for its terms and attribution requirements.

Project code and documentation licensing will be specified separately.

---

**Author:** Samprath Shanbhag  
**GitHub:** https://github.com/samprathshanbhag
