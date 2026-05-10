# E-commerce User Behavior Funnel Analysis (SQL-BigQuery)
## 1. Project Information
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
<img width="740" height="452" alt="image" src="https://github.com/user-attachments/assets/cb90244f-14a1-4c46-b74f-3632e2823f00" />

## 4. Analysis & Queries
### 4.1 Monthly Metrics (Jan–Mar 2017)
Query 01: calculate total visit, pageview, transaction for Jan, Feb and March 2017 (order by month)

<img width="650" height="350" alt="image" src="https://github.com/user-attachments/assets/535258e9-0621-4747-90a0-13bbaf1ca69e" />

💡 Queries result:
<img width="650" height="150" alt="image" src="https://github.com/user-attachments/assets/79e9bd4d-6a4e-4b52-a8b8-a23a280378e1" />

In Q1 2017, traffic shows a slight dip in February before recovering in March. Visits decreased from 64,694 (Jan) to 62,192 (Feb), then increased to 69,931 (Mar), with pageviews following a similar pattern. Notably, transactions grew steadily, reaching 993 in March, the highest among the three months.

This indicates that while traffic fluctuated, conversion performance improved over time, especially in March. The disproportionate growth in transactions vs visits suggests better traffic quality or improved user purchase behavior, not just higher volume.

### 4.2 Bounce Rate by Traffic Source (July 2017)
Query 02: Bounce rate per traffic source in July 2017 (Bounce_rate = num_bounce/total_visit) (order by total_visit DESC)

<img width="850" height="330" alt="image" src="https://github.com/user-attachments/assets/00fab761-067f-4f82-9ce1-04301989f309" />

💡 Queries result:

### 4.3 Revenue by Traffic Source (June 2017)

<img width="778" height="688" alt="image" src="https://github.com/user-attachments/assets/1dc5cff4-f4ec-4690-b3b5-d6d39bb1445a" />

💡 Queries result:

### 4.4 Conversion Rate by Traffic Source (2017)

<img width="585" height="460" alt="image" src="https://github.com/user-attachments/assets/63699593-9aef-4ac8-8cb8-434b79e962d4" />

💡 Queries result:

### 4.5 Pageviews by Purchaser Type (June–July 2017)
### 4.6 Transactions per Purchasing User (July 2017)
### 4.7 Revenue Contribution by Device
### 4.8 Product Co-purchase Analysis (July 2017)
### 4.9 Funnel Analysis (Jan–Mar 2017)

### 4.10 Weekly Revenue & Cumulative Revenue (May–July 2017)

<img width="589" height="465" alt="image" src="https://github.com/user-attachments/assets/6d54a655-cf1f-4954-a78f-115d256848b5" />



