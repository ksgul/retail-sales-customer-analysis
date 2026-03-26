# Retail Sales & Customer Behaviour Analysis (End-to-End Power BI Project)

# Description:
This project analyses a dataset of 500k+ retail transactions to extract business insights regarding sales performance and customer loyalty.
This dataset contains all purchases made for an online retail company based in the UK during an eight-month period.

## 1. Data Pipeline & Preparation

### Step 1: Excel Preprocessing. Fixed product naming inconsistencies and removed leading/trailing spaces for accurate grouping, transformed data type.

### Step 2: Python Data Cleaning (every step is described in 'sales.ipynb' file).

- Handled missing values in Description and CustomerID.
- Converted data types (Dates, Numeric) for proper calculation.
- Filtered out returns (negative quantities) to ensure revenue accuracy.

### Step 3: Data Segmentation. Split the dataset into two specialized files:

- sales_clean.csv: Optimized for general sales trends and product performance.
- sales_customers_clean.csv: Focused on identifiable customer (with known IDs) transactions for loyalty and behavioural analysis.

## 2. Business Insights & Dashboards
_(Please Note: The currency of price was not specified, therefore I've decided to omit it. It would be logical to add pounds (£) as currency based on company's origin.)_

### Dashboard 1: Sales Performance
- Focus: Revenue trends, Top Markets, and Product Performance.
- Key Metrics: Total Revenue, Sales per Day/Month/Year, and Top 5 Bestsellers.
- Interactive Features: Integrated Slicers for Date and Country to allow more detailed exploration of regional markets.

<img width="1379" height="778" alt="Image" src="https://github.com/user-attachments/assets/eae873e1-4647-476b-aaf1-492f5a93a3ef" />

### Dashboard 2: Customer Behaviour (sales_clients.png)
- Focus: Loyalty, Retention, and Purchasing Patterns.
- Key Metrics: Average Check, Loyal Customer count (Returns within 35 days), and Purchase Count distribution.
- Visual Analysis: Includes a Retention Comparison and a monthly trend of returning customers to identify seasonal loyalty peaks.

<img width="1376" height="774" alt="Image" src="https://github.com/user-attachments/assets/439900da-8a45-49e7-83d2-a6d13ccce68b" />

### Main Highlights:
_**Sales:**_
- The main market (85% of all sales) is UK (main selling season is autumn). _This may be due to more aggressive marketing in the UK (not only online)._
- There are 69 unpopular products (only one purchase over time). _Solutions: marketing or removing from the shop._
- Top-5 best-selling products is the key to business success. _The business should be focused on those or similar products._
- There is the difference between best-selling products in every country. _It may be useful when deciding on main marketing focus._ 
- 1/6 (16.28%) of all customers are anonymous. _Information is more useful for the business when it is possible to track customer behaviour._

_**Clients:**_
- Most identified clients have done only one purchase. _Low loyalty rate (869 clients from 4339 customers) indicates the need to change the selling strategy._
- Most loyal customers return in about 1 month (approx. 35 days), clients with 2 - 5 purchases came again 2.5 times less often - in around 3 month (approx. 89 days). _It is a signal to look deeper in offer. Maybe it is a time to change something? Maybe it would be useful to ask clients to fill a quick questionnaire?_
- Top customer have spent around 280K. It's 3,6 times more than top 10 spending customer. _To minimise the difference, it is useful to look deeper into their purchases and personalise offers. It can stimulate client to return and become more loyal to spend more._ 
- Customers eager to return in November and December. It can be due to celebrations like Halloween or Christmas. _To stimulate customer loyalty, it can be useful to do celebratory offers (for example, before Christmas or on Valentines Day, etc.)._

# 3. Technical Stack
- Data Cleaning: Excel, Python (Pandas).
- Visualization: Power BI (DAX, Interactive Slicers, Data Modelling).
- Dataset: [Kaggle Online Retail Dataset](https://www.kaggle.com/datasets/vijayuv/onlineretail).
