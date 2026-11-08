# Retail360
End-to-End Business Intelligence, Customer Analytics &amp; Workflow Automation Platform
# Retail360 – End-to-End Business Intelligence, Customer Analytics & Workflow Automation Platform

**Turning Retail Data into Actionable Business Intelligence**

---

## 1. Project Overview

Retail360 is an end-to-end Business Intelligence and Analytics platform designed to transform raw e-commerce data into meaningful business insights and actionable recommendations.

The project uses the Brazilian E-Commerce Public Dataset by Olist to analyse sales performance, customer purchasing behaviour, product performance, regional trends and operational efficiency.

By integrating Python-based data processing, PostgreSQL, SQL analytics, Power BI dashboards, Streamlit applications and n8n workflow automation, Retail360 demonstrates how businesses can build a structured, automated and data-driven decision-making system.

Unlike a traditional dashboard project, Retail360 covers the complete analytics lifecycle, including data acquisition, exploration, cleaning, transformation, storage, analysis, visualisation, reporting and workflow automation.

**Primary Objective:** To develop a scalable and reproducible retail analytics solution that helps management understand business performance, identify operational challenges and make evidence-based decisions.

---

## 2. Business Problem

Growing retail and e-commerce businesses generate large volumes of transactional data. However, having access to data does not automatically translate into better business decisions.

Management may face several challenges:

- Limited visibility into sales trends and overall business performance.
- Difficulty understanding customer purchasing behaviour and retention.
- Inability to identify high-value, frequent and inactive customers.
- Difficulty identifying high-performing and underperforming products.
- Inconsistent sales performance across geographical regions.
- Limited visibility into delivery performance and customer satisfaction.
- Lack of structured monitoring for important business KPIs.
- Time-consuming manual data processing and report generation.
- Lack of automated reporting and performance alerts.

Retail360 addresses these challenges by building an integrated analytics platform that processes business data, identifies trends, monitors performance, generates reports and automates repetitive analytical tasks.

---

## 3. Business Questions & Analytical Objectives

Retail360 aims to answer important business questions across six analytical areas.

### A. Sales Performance Analytics

- What is the total sales revenue?
- How are revenue and order volumes changing over time?
- What is the Average Order Value (AOV)?
- Which months generate the highest sales?
- Which regions contribute most to overall revenue?
- How do freight charges compare with product revenue?
- What are the month-over-month and year-over-year growth trends?

### B. Customer Intelligence

- Who are the most valuable customers?
- Which customers make repeat purchases?
- What percentage of customers return to make another purchase?
- Which customers have become inactive?
- Which customer segments contribute the most revenue?
- How does customer purchasing behaviour change over time?
- What does cohort analysis reveal about customer retention?
- How can customers be segmented using RFM analysis?

### C. Product Performance Analytics

- Which products generate the highest revenue?
- Which product categories perform best?
- Which products have high sales volumes?
- Which categories contribute most to total revenue?
- How does product performance vary across regions?
- Which products receive poor customer review scores?
- Are there products with high sales but low profitability, where cost data is available?

### D. Regional Analytics

- Which Brazilian states and cities generate the highest revenue?
- Which regions have the highest order volumes?
- How is customer distribution spread geographically?
- Which regions experience longer delivery durations?
- Are there geographical differences in customer satisfaction?

### E. Operational Analytics

- What is the average delivery duration?
- What percentage of orders are delivered late?
- Which regions experience the most delivery delays?
- What are the major order cancellation patterns?
- How do delivery experiences relate to customer review scores?
- How does order fulfilment performance change over time?

### F. Business Performance Monitoring

- Has revenue declined compared with the previous period?
- Are order cancellations increasing?
- Is delivery performance deteriorating?
- Which KPIs require management attention?
- Can recurring reports and business performance monitoring be automated?

The project will use analytical findings to develop evidence-based business recommendations rather than assuming conclusions before analysing the data.

---

## 4. Dataset – Brazilian E-Commerce Public Dataset by Olist

### Dataset Overview

Retail360 uses the **Brazilian E-Commerce Public Dataset by Olist**, a publicly available real-world e-commerce dataset published on Kaggle.

Olist is a Brazilian e-commerce platform that connects merchants with customers through an online marketplace.

The dataset contains approximately 100,000 orders placed between 2016 and 2018. It provides anonymised information about customers, orders, products, sellers, payments, reviews and delivery operations.

This dataset provides a realistic foundation for studying e-commerce transactions, customer purchasing patterns, sales performance and operational efficiency.

**Dataset Source:** [Brazilian E-Commerce Public Dataset by Olist – Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

### Dataset Components

The dataset consists of nine interconnected CSV files:

| Dataset | Description |
|---|---|
| Customers | Customer identifiers, zip code prefixes, cities and states. |
| Orders | Order IDs, customer IDs, order status and purchase, approval, shipping and delivery timestamps. |
| Order Items | Products purchased in each order, seller information, item prices and freight values. |
| Products | Product identifiers, categories, dimensions and weight. |
| Payments | Payment methods, payment values, instalments and transaction information. |
| Reviews | Customer review scores, review comments and timestamps. |
| Sellers | Seller identifiers and geographical information. |
| Geolocation | Brazilian zip code prefixes and geographical coordinates. |
| Category Translation | Portuguese product category names and their English translations. |

### Why This Dataset?

The Olist dataset was selected because it contains multiple interconnected datasets rather than a single flat transaction file.

This makes it suitable for demonstrating:

- Relational database design and SQL joins.
- Sales and revenue analysis.
- Customer segmentation and purchasing behaviour.
- Product and category performance analysis.
- Payment method analysis.
- Regional and geographical analysis.
- Order fulfilment and delivery performance.
- Customer satisfaction analysis.
- Customer retention and cohort analysis.

### Dataset Limitations

The dataset has certain limitations that must be considered during analysis:

- Actual product acquisition costs are not available.
- Actual discount amounts are not directly provided.
- Dedicated product return and refund records are not available.
- The dataset represents historical transactions rather than current e-commerce activity.
- Customer and seller information is anonymised.

Therefore, actual profitability, discount effectiveness and product return analysis will not be presented as real observations without appropriate additional data.

Any external or simulated data introduced during development will be clearly documented and distinguished from actual dataset observations.

---

## 5. Project Objectives

The primary objectives of Retail360 are:

1. Develop a reusable Python-based ETL pipeline.
2. Perform structured data cleaning and validation.
3. Design a relational PostgreSQL database.
4. Perform advanced SQL-based business analytics.
5. Conduct exploratory data analysis using Pandas and NumPy.
6. Implement customer segmentation and cohort analysis.
7. Develop interactive Power BI dashboards.
8. Generate automated Excel and PDF reports.
9. Build a multi-page Streamlit analytics application.
10. Automate repetitive processes using n8n.
11. Implement data quality monitoring and KPI alerts.
12. Generate actionable business insights and recommendations.

---

## 6. Key Project Functionalities

### 6.1 Data Acquisition & Processing

- Import CSV and Excel datasets.
- Validate input files and expected columns.
- Detect missing values and duplicate records.
- Standardise data types and date formats.
- Clean and transform datasets.
- Generate derived analytical metrics.
- Maintain ETL execution logs.
- Handle processing errors.

### 6.2 Database Management & SQL Analytics

- Design relational database tables.
- Implement primary and foreign keys.
- Establish table relationships and constraints.
- Store processed data in PostgreSQL.
- Perform SQL-based business analysis.
- Use joins, subqueries, CTEs and window functions.
- Create analytical views and reporting tables.
- Design a star schema for Power BI.

### 6.3 Business Analytics

- Revenue and sales trend analysis.
- Customer segmentation using RFM.
- Repeat purchase and retention analysis.
- Customer cohort analysis.
- Product and category performance.
- Regional sales analysis.
- Payment behaviour analysis.
- Delivery and operational performance.
- Customer satisfaction analysis.

### 6.4 Power BI Dashboards

Three interactive dashboards are planned.

**Dashboard 1 – Executive Performance**
- Revenue and order volume.
- Average Order Value.
- Monthly and yearly growth.
- Regional performance.
- Business KPI monitoring.

**Dashboard 2 – Customer Intelligence**
- RFM customer segmentation.
- Repeat purchase behaviour.
- Customer retention.
- Cohort analysis.
- Customer lifetime value estimates.

**Dashboard 3 – Product & Operations Intelligence**
- Product and category performance.
- Payment analysis.
- Delivery performance.
- Customer satisfaction.
- Operational trends.

Features will include DAX measures, Power Query transformations, slicers, drill-through and interactive visualisations.

### 6.5 Automated Reporting

**Excel Reports**
- Executive summary.
- Sales performance.
- Customer analysis.
- Product performance.
- Regional performance.

**PDF Reports**
- Management summary.
- Important business KPIs.
- Analytical charts.
- Key findings.
- Business recommendations.

Reports will be generated programmatically using processed analytical data.

### 6.6 Streamlit Application

The Streamlit application will provide an interactive interface where users can:

- Upload CSV and Excel files.
- Validate uploaded datasets.
- Execute the ETL pipeline.
- View data quality summaries.
- Explore business KPIs.
- View interactive charts.
- Explore analytical findings.
- Generate Excel and PDF reports.
- Download generated reports.

### 6.7 n8n Workflow Automation

n8n will act as the workflow orchestration layer.

Planned automation workflows include:

**Workflow 1 – Automated ETL Pipeline**
- Trigger Python ETL execution.
- Validate pipeline output.
- Load processed data into PostgreSQL.
- Generate execution summaries.
- Send success or failure notifications.

**Workflow 2 – Data Quality Monitoring**
- Check missing values.
- Detect duplicate records.
- Identify invalid data.
- Monitor processing failures.
- Send data quality notifications.

**Workflow 3 – Automated Monthly Business Reports**
- Schedule monthly reporting.
- Execute SQL queries.
- Retrieve analytical results.
- Generate Excel and PDF reports.
- Deliver reports through email.

**Workflow 4 – Business Performance Alerts**
- Monitor revenue changes.
- Track order volume.
- Monitor cancellation rates.
- Track delivery performance.
- Trigger notifications when configurable thresholds are exceeded.

**Workflow 5 – Scheduled Data Processing**
- Schedule recurring ETL jobs.
- Update analytical tables.
- Refresh processed datasets.
- Generate updated reports.
- Maintain execution history.

Python will handle the actual data processing, while n8n will coordinate execution, scheduling, conditional logic and notifications.

---

## 7. Project Workflow & Architecture

Retail360 follows a modular data engineering and business intelligence architecture.

```text
              RAW DATA SOURCES
             Olist CSV / Excel Files
                      |
                      v
              DATA ACQUISITION
                Python + Pandas
                      |
                      v
               DATA EXPLORATION
             Pandas + NumPy + Jupyter
                      |
                      v
               DATA VALIDATION
         Schema / Missing Values / Duplicates
                      |
                      v
             DATA TRANSFORMATION
                 Python + Pandas
                      |
                      v
              POSTGRESQL DATABASE
              Relational Data Storage
                      |
                      v
              BUSINESS ANALYTICS
                 Python + SQL
                      |
                      v
             ANALYTICAL DATA MODEL
                   Star Schema
                      |
             +--------+--------+
             |        |        |
             v        v        v
          POWER BI STREAMLIT REPORTING
          Dashboards Application Excel / PDF
             |        |        |
             +--------+--------+
                      |
                      v
              n8n AUTOMATION
         Scheduling / Monitoring / Reporting
                / Notifications
                      |
                      v
             BUSINESS INSIGHTS
           & MANAGEMENT DECISIONS
```

### Workflow Explanation

| Stage | Process | Technologies |
|---|---|---|
| 1 | Data acquisition | Python, Pandas |
| 2 | Data exploration | Pandas, NumPy, Jupyter Notebook |
| 3 | Data validation | Python, Pandas |
| 4 | Data cleaning and transformation | Python, Pandas, NumPy |
| 5 | Data storage | PostgreSQL, SQLAlchemy, Psycopg2 |
| 6 | Business analytics | SQL, Python |
| 7 | Analytical data modelling | PostgreSQL, Power Query |
| 8 | Business dashboards | Power BI, DAX |
| 9 | Interactive application | Streamlit, Plotly |
| 10 | Excel reporting | OpenPyXL |
| 11 | PDF reporting | Python PDF generation library |
| 12 | Workflow automation | n8n, Docker |
| 13 | Version control | Git, GitHub |

Power BI and Streamlit will function as separate interfaces using the same processed analytical data. Data processing logic will not be unnecessarily duplicated.

---

## 8. Technology Stack

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Data Processing | Pandas, NumPy |
| Database | PostgreSQL |
| Database Connectivity | SQLAlchemy, Psycopg2 |
| Query Language | SQL |
| Business Intelligence | Microsoft Power BI |
| Data Modelling & Calculations | Power Query, DAX |
| Application Development | Streamlit |
| Visualisation | Plotly, Power BI |
| Excel Reporting | OpenPyXL |
| PDF Reporting | Python PDF libraries |
| Workflow Automation | n8n |
| Containerisation | Docker |
| Version Control | Git, GitHub |
| Development Environment | VS Code, Jupyter Notebook |

---

## 9. Repository Structure

The project follows a modular directory structure to maintain code organisation, reproducibility and maintainability.

```text
Retail360/
│
├── data/
│   ├── raw/
│   ├── processed/
│   └── external/
│
├── notebooks/
│   ├── 01_data_understanding.ipynb
│   ├── 02_data_cleaning.ipynb
│   ├── 03_sales_analysis.ipynb
│   └── 04_customer_analysis.ipynb
│
├── src/
│   ├── ingestion/
│   ├── cleaning/
│   ├── transformation/
│   ├── validation/
│   ├── analytics/
│   └── reporting/
│
├── sql/
│   ├── schema/
│   ├── staging/
│   ├── transformations/
│   └── business_queries/
│
├── powerbi/
│   ├── executive_dashboard/
│   ├── customer_dashboard/
│   └── product_dashboard/
│
├── app/
│   ├── app.py
│   └── pages/
│
├── n8n/
│   ├── workflows/
│   └── documentation/
│
├── reports/
├── tests/
├── logs/
├── config/
│
├── requirements.txt
├── .gitignore
└── README.md
```

Large raw datasets, generated temporary files, credentials and environment-specific configuration files will be excluded from GitHub where appropriate.

---

## 10. Engineering Practices

Retail360 aims to follow professional software development practices:

- Modular and reusable Python code.
- Meaningful variable and function names.
- Exception handling and execution logging.
- Data validation and quality checks.
- Configuration-based environment management.
- Database constraints and appropriate indexing.
- SQL scripts maintained separately.
- Unit testing and pipeline validation.
- Git-based version control.
- Clear technical documentation.
- Reproducible project setup instructions.
- Secure handling of database credentials and API keys.

---

## 11. Expected Project Deliverables

The final project will include:

1. Complete GitHub repository.
2. Documented Python ETL pipeline.
3. PostgreSQL relational database.
4. Analytical SQL query collection.
5. Python exploratory data analysis notebooks.
6. Three interactive Power BI dashboards.
7. Automated Excel reporting system.
8. Automated PDF reporting system.
9. Multi-page Streamlit application.
10. Multiple functional n8n workflows.
11. Data quality monitoring system.
12. Automated reporting and notification workflows.
13. Technical and architecture documentation.
14. Business findings and recommendations.
15. Project screenshots and demonstrations.

---

## 12. Project Development Status

<ins>Current Status: Initial Development – In Progress</ins>

| Module | Status |
|---|---|
| Project Planning & Architecture | Completed |
| Dataset Acquisition | Completed |
| GitHub Repository Setup | In Progress |
| Data Acquisition & Exploration | Pending |
| Python ETL Pipeline | Pending |
| PostgreSQL Database | Pending |
| Business Analytics | Pending |
| Power BI Dashboards | Pending |
| Automated Reporting | Pending |
| Streamlit Application | Pending |
| n8n Workflow Automation | Pending |
| Final Documentation | Pending |

Features will be marked as completed only after implementation and testing.

---

## 13. Project Vision

Retail360 aims to demonstrate how raw transactional data can be transformed into a structured business intelligence solution through data engineering, analytical thinking, visualisation and workflow automation.

The project focuses on building a practical, reproducible and maintainable analytics platform that supports data-driven retail business decisions.

**Retail360 – Turning Retail Data into Business Intelligence.**
