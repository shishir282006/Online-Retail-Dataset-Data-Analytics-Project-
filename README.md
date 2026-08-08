# 📊 Online Retail Dataset (UCI Machine Learning Repository)

📌 Project Overview
This project involves the completion, cleaning, and preprocessing of the Online Retail Dataset from the UCI Machine Learning Repository (archive.ics.uci.edu in Bing).
The dataset contains transactional data from a UK-based online retail store between 01/12/2010 and 09/12/2011, focusing on sales of gift items.

---

The primary goal of this project was to:

Handle missing, duplicate, and inconsistent values.

Prepare the dataset for exploratory data analysis (EDA) and machine learning tasks.

Generate insights into customer behavior, product performance, and sales trends.

---

## 📂 Dataset Information
Source: UCI Machine Learning Repository

Records: ~541,909 transactions

##Features:

### InvoiceNo – Transaction ID

### StockCode – Product code

### Description – Product description

### Quantity – Number of items purchased

### InvoiceDate – Date and time of transaction

### UnitPrice – Price per item

### CustomerID – Unique customer identifier

### Country – Country of customer

---

## 🛠️ Data Cleaning & Preprocessing Steps
01
### Load raw dataset
Imported the Online Retail dataset from UCI repository into Python using pandas.
02
### Handle missing values
Removed rows with missing CustomerID and Description to ensure data integrity.
03
### Remove duplicates
Dropped duplicate records to avoid bias in analysis.
04
### Filter invalid entries
Excluded transactions with negative or zero Quantity and UnitPrice.
05
### Convert data types
Transformed InvoiceDate into datetime format and standardized numeric fields.
06
### Feature engineering
Created new features like TotalAmount = Quantity × UnitPrice for revenue analysis.
07
### Final dataset export
Saved the cleaned dataset for further analysis and machine learning tasks.
## 📈 Applications
Exploratory Data Analysis (EDA): Customer segmentation, product popularity, seasonal trends.

---

## Machine Learning:

Customer lifetime value prediction

Market basket analysis (association rules)

Clustering for customer segmentation

---

## ⚙️ Tools & Libraries
Python: pandas, numpy, matplotlib, seaborn

Jupyter Notebook for analysis and documentation

Excel/CSV for dataset storage

---

## 🚀 How to Use
Clone this repository.

Open the Jupyter Notebook OnlineRetail_Cleaning.ipynb.

Run the cells step by step to reproduce the cleaning process.

Use the cleaned dataset (OnlineRetail_Cleaned.csv) for analysis or ML tasks.

---

## 📜 License
This dataset is provided by the UCI Machine Learning Repository for research and educational purposes.
