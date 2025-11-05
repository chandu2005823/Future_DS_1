# FUTURE_DS_01 — Business Sales Dashboard

## 📊 Task 1: Business Sales Dashboard from E-commerce Data

### 🔹 Task Overview
Analyze e-commerce sales data to identify **best-selling products**, **sales trends**, and **high-revenue categories** using **Power BI**.

This repository documents the completion of **Task 1** for the **Future Interns – Data Science & Analytics Internship**.  
The project aims to transform raw e-commerce data into meaningful business insights through data cleaning, DAX measures, and interactive visualizations.

---

## 🧠 Introduction
The goal of this project was to explore and analyze an e-commerce dataset to help businesses understand:
- Which products and categories generate the highest revenue
- When sales peak during the year
- How different regions or customer segments perform

The outcome is a **fully interactive Power BI dashboard** designed for data-driven decision-making.

---

## 🧩 Skills Gained
- 📉 Data Cleaning and Transformation (Power Query)
- 🧮 DAX (Data Analysis Expressions)
- 📆 Time Series & Trend Analysis
- 🎯 Business Storytelling and Visualization

---

## 🛠️ Tools Used
- **Microsoft Power BI Desktop**
- **Excel / CSV Dataset**
- **Power Query Editor**

---

## 📈 Deliverable
An **interactive Power BI dashboard** with:
- KPIs for Total Sales, Total Profit, and Quantity Sold  
- Charts showing Category and Sub-Category performance  
- Yearly sales trends and regional comparisons  
- Dynamic slicers for Month and Quarter filtering  

---


---

## 💡 Key Insights
- **Total Sales:** 2.30M | **Total Profit:** 286.4K | **Total Quantity:** 38K  
- Technology category contributes the highest revenue (~36%).  
- Steady growth in sales from **2011 to 2014**, peaking in 2014.  
- East and South regions show nearly equal sales share (~46% each).  
- Average Order Value ≈ ₹45K indicates consistent customer spending.  

---

## 🧮 DAX Measures Used
```DAX
Total Sales = SUM('Retail_Clean'[Revenue])
Total Profit = SUM('Retail_Clean'[Profit])
Total Quantity = SUM('Retail_Clean'[Quantity])
Distinct Orders = DISTINCTCOUNT('Retail_Clean'[Invoice])
Average Order Value = DIVIDE([Total Sales], [Distinct Orders], 0)
