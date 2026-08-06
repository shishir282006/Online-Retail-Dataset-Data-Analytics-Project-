🛒 Online Retail Dataset
 README
📌 Overview


The Online Retail Dataset is a transactional dataset containing purchase records from a UK-based online retail store. It is widely used for data analysis, machine learning, and business intelligence projects. The dataset provides insights into customer behavior, product performance, and sales trends.

📂 Dataset Information

Source: UCI Machine Learning Repository

Records: ~500,000 transactions

Time Period: 01/12/2009 – 09/12/2011

Format: CSV

📑 Features (Columns)
Column Name	Description
InvoiceNo	Unique identifier for each transaction (numeric, may start with "C" for cancellations).
StockCode	Product/item code.
Description	Name of the product.
Quantity	Number of items purchased per transaction.
InvoiceDate	Date and time of the transaction.
UnitPrice	Price per item (£).
CustomerID	Unique identifier for each customer.
Country	Country where the customer resides.


🎯 Use Cases
Customer Segmentation (RFM analysis, clustering)

Market Basket Analysis (association rules, recommendation systems)

Sales Forecasting (time series analysis)

Data Cleaning & Preprocessing Practice

Visualization Projects (dashboards in Power BI, Tableau, or Python libraries)

⚠️ Data Quality Notes
Contains missing values (especially in CustomerID).

Includes canceled transactions (marked with "C" in InvoiceNo).

Some records may have negative quantities (returns).

Requires data cleaning before analysis.

🚀 Getting Started
Load the dataset:

python
import pandas as pd
df = pd.read_csv("OnlineRetail.csv", encoding="ISO-8859-1")
Explore basic info:

python
df.info()
df.head()
Handle missing values & cancellations:

python
df = df.dropna(subset=["CustomerID"])
df = df[~df["InvoiceNo"].astype(str).str.startswith("C")]
📊 Example Analysis
Top 10 Products by Sales

Revenue by Country

Monthly Sales Trends

Customer Lifetime Value (CLV)

📜 License
This dataset is provided by the UCI Machine Learning Repository for research and educational purposes.
