# E-commerce User Behavior Funnel Analysis (SQL-BigQuery)
## 1. Project Information
- Author: Linh Ta
- Date: March 2025
- Tools: SQL (BigQuery)
## 2. Background & Objective
### 2.1 Overview
This project analyzes the Google Analytics sample dataset in BigQuery to extract insights related to user sessions, traffic sources, transactions, and product interactions.
### 2.2 Objectives
- Aggregate session-level metrics (visits, pageviews, transactions)
- Analyze bounce rate and conversion rate by traffic source
- Evaluate revenue performance across time and device categories
- Compare user behavior between purchasers and non-purchasers
- Identify co-purchased products
- Analyze user actions across funnel stages 
## 3. Dataset Description
### 3.1 Data Source
- Source: Google Analytics sample dataset
- Table: bigquery-public-data.google_analytics_sample.ga_sessions_*
- Reference: https://support.google.com/analytics/answer/3437719?hl=en
### 3.2 Data Structure (Relevant Fields)
<img width="605" height="352" alt="image" src="https://github.com/user-attachments/assets/cb90244f-14a1-4c46-b74f-3632e2823f00" />

## 4. Analysis & Queries
### 4.1 Monthly Metrics (Jan–Mar 2017)
Query 01: calculate total visit, pageview, transaction for Jan, Feb and March 2017 (order by month)

<img width="278" height="141" alt="image" src="https://github.com/user-attachments/assets/535258e9-0621-4747-90a0-13bbaf1ca69e" />

💡 Queries result:
<img width="309" height="53" alt="image" src="https://github.com/user-attachments/assets/79e9bd4d-6a4e-4b52-a8b8-a23a280378e1" />

In Q1 2017, traffic shows a slight dip in February before recovering in March. Visits decreased from 64,694 (Jan) to 62,192 (Feb), then increased to 69,931 (Mar), with pageviews following a similar pattern. Notably, transactions grew steadily, reaching 993 in March, the highest among the three months.

This indicates that while traffic fluctuated, conversion performance improved over time, especially in March. The disproportionate growth in transactions vs visits suggests better traffic quality or improved user purchase behavior, not just higher volume.

