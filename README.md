# Ubuntu Bank Financial Crime Risk Assessment Platform

## Overview

This repository contains an end-to-end cloud data engineering solution built to support financial crime detection within a simulated retail banking environment.

The platform ingests operational banking data from Oracle Autonomous Database into Azure Databricks, processes it through a Medallion Architecture using Delta Lake and Unity Catalog, and delivers curated analytical datasets to Microsoft Power BI.

Rather than relying on opaque machine learning models, the solution implements a transparent, rule-based risk engine that produces explainable fraud scores for customers, merchants, devices and financial crime investigations.

The project demonstrates the design and implementation of a modern enterprise data platform using scalable ETL pipelines, governed data assets, dimensional modelling and business-focused analytics.

---

## Architecture Overview

The platform follows a layered Medallion Architecture.

```
Oracle Autonomous Database
            │
            ▼
Metadata-Driven Bronze Ingestion
            │
            ▼
Bronze Delta Tables
            │
            ▼
Silver Data Transformation
            │
            ▼
Gold Business Marts
            │
            ▼
Explainable Risk Engine
            │
            ▼
Power BI Semantic Model
            │
            ▼
Interactive Fraud Intelligence Dashboards
```

---

## Technology Stack

| Component | Technology |
|------------|------------|
| Cloud Platform | Microsoft Azure |
| Source Database | Oracle Autonomous Database |
| Data Engineering | Azure Databricks |
| Data Lake | Delta Lake |
| Data Governance | Unity Catalog |
| Programming | Python, PySpark, SQL |
| Reporting | Microsoft Power BI |
| Version Control | Git & GitHub |

---

## Data Pipeline

The solution is organised into three logical layers.

### Bronze

The Bronze layer performs metadata-driven ingestion from Oracle Autonomous Database into Delta Lake while preserving the raw source data.

Key processes include:

- Dynamic table ingestion
- Incremental loading
- Pipeline auditing
- Data quality validation
- Historical data retention

### Silver

The Silver layer standardises and enriches the raw datasets.

Transformations include:

- Data cleansing
- Standardisation
- Feature engineering
- Slowly Changing Dimension (Type 2)
- Fraud indicator generation
- Referential integrity validation

### Gold

The Gold layer produces business-ready datasets designed specifically for fraud analytics and executive reporting.

Analytical marts include:

- Enterprise Risk Assessment
- Customer Risk Assessment
- Financial Crime Investigation
- Merchant Intelligence
- Device Intelligence
- Geographic Intelligence

---

## Fraud Risk Engine

The platform implements a rule-based risk scoring framework that provides transparent and explainable fraud assessments.

Risk scores are calculated using multiple business dimensions, including:

- Enterprise Risk Score
- FIU Risk Score
- Merchant Risk Score
- Device Risk Score
- Transaction Velocity
- Beneficiary Exposure

Each score can be traced back to the business rules used during calculation, providing complete auditability and explainability.

---

## Power BI Dashboards

### Executive Command Centre

Provides an executive view of fraud exposure, customer risk distribution, transaction activity and operational KPIs.

---

### Enterprise Customer Risk

Analyses customer behaviour, risk segmentation and suspicious transaction activity.

---

### Financial Crime Investigation


Supports fraud investigators with detailed customer-level intelligence and investigation prioritisation.

---

### Device Fraud Intelligence

Identifies suspicious devices, rooted devices and emulator-based fraud.

---

### Merchant Intelligence

Analyses merchant behaviour, transaction concentration and merchant risk.

---

### Geographic Intelligence


Visualises fraud activity geographically to identify regional hotspots and emerging trends.

---

### Investigation Workbench

Provides investigators with a consolidated view of customer activity, transactions and explainable fraud indicators.

---

## Project Highlights

- Metadata-driven ingestion framework
- Oracle Autonomous Database integration
- Azure Databricks notebooks
- Delta Lake Medallion Architecture
- Unity Catalog governance
- PySpark transformation pipelines
- Slowly Changing Dimensions (Type 2)
- Explainable rule-based fraud scoring
- Gold analytical marts
- Interactive Power BI dashboards

---

## Repository Structure

```
ubuntu-bank-financial-crime-platform
│
├── architecture/
│
├── documentation/
│
├── images/
│
├── notebooks/
│   ├── bronze/
│   ├── silver/
│   └── gold/
│
├── powerbi/
│
├── sql/
│
└── README.md
```

---

## Skills Demonstrated

- Azure Databricks
- Oracle Autonomous Database
- Delta Lake
- Unity Catalog
- PySpark
- SQL
- Data Engineering
- Medallion Architecture
- Metadata-Driven ETL
- Data Modelling
- Slowly Changing Dimensions (Type 2)
- Fraud Analytics
- Microsoft Power BI

---

## Future Enhancements

Potential improvements include:

- Real-time fraud detection using streaming ingestion
- Machine learning-based anomaly detection
- Automated CI/CD deployment
- Event-driven fraud alerting

---

## Author

**Kulani Baloyi**

Data Engineer | Azure Data Engineer | Data Analytics Engineering


