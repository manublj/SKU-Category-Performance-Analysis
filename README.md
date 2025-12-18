# 📦 Maximizing Profitability Through SKU & Category Sales Analysis  
### A Deep Dive into Amazon E-Commerce Data

## 📌 Project Overview
This project performs an **SKU- and Category-level sales analysis** on an Amazon e-commerce dataset using Python.  
The objective is to uncover **revenue concentration, demand patterns, and operational insights** that can support better inventory planning, fulfillment decisions, and category prioritization.

The analysis is entirely **exploratory and diagnostic in nature** (EDA + business analytics).  
No predictive models are used — the focus is on **understanding what drives performance** in transactional sales data.

---

## 🎯 Objectives
- Clean and prepare raw e-commerce sales data for analysis  
- Understand overall sales performance using high-level KPIs  
- Analyze **SKU-level and category-level revenue contribution**  
- Identify **top-performing and underperforming SKUs**  
- Evaluate **revenue concentration** using Pareto (80/20) analysis  
- Examine **time-based demand patterns** (daily and weekly trends)  
- Study **fulfillment methods** and **B2B vs B2C** sales distribution  
- Generate **actionable business insights** for decision-making  

---

## 📊 Dataset
- **Source:** Amazon E-commerce Sales Dataset (Kaggle)  
- **Time Period:** April 01, 2022 – June 29, 2022  
- **Granularity:** Transaction-level sales records  

### Key Columns
- `SKU`, `Category`
- `Date`
- `Qty`, `Amount`
- `Fulfilment`
- `B2B`
- Additional product and logistics attributes

---

## 🛠️ Tools & Libraries
- **Python**
- `pandas` — data manipulation & aggregation  
- `numpy` — numerical operations  
- `matplotlib`, `seaborn` — data visualization  

---

## 🔍 Analysis Approach

### 1. Data Preparation
- Standardized column names and data types  
- Converted date fields to datetime format  
- Ensured numeric consistency for quantity and revenue  
- Removed duplicates and invalid records  
- Created **derived analytical metrics** (e.g., revenue per unit, day of week)

### 2. Exploratory Data Analysis (EDA)
- High-level KPIs: total revenue, total units, unique SKUs and categories  
- Daily revenue and quantity trends  
- Category-level and SKU-level revenue analysis  
- Revenue vs quantity comparison across SKUs  
- Weekly demand patterns using heatmaps  

### 3. Revenue Concentration
- Pareto (80/20) analysis to identify how many SKUs contribute to the majority of revenue  
- Identification of high-impact SKUs for prioritization  

### 4. Operational Insights
- Fulfillment method distribution  
- B2B vs B2C revenue contribution  
- Identification of underperforming SKUs (bottom 5% by revenue)  

---

## 💡 Key Insights (Summary)
- Based on the analysis, we can draw some preliminary insights about the Q2 2022 performance of Amazon India:
- The total revenue for Q2 2022 decreased by -18.77% from April to June, with May revenue experiencing a -9.06% decrease from April, and June revenue seeing a -10.68% decrease from May, which is a cause of concern.
- The revenue is dominated by the product category "Set," which accounts for 49.88% of total revenue, followed by kurta with 27.09% and Western Dress with 14.28%.
- The top 5 product categories by average price in dollars are Set (\$9.43), Saree (\$9.14), Western Dress (\$8.75), Ethnic Dress (\$8.26), and Top (\$6.09), indicating that these products are high-value orders.
- The total number of cancelled and returned orders was 49,178, which represents 17.53% of all orders. Of these, 14.22% were cancelled and 1.64% were returned.
- The average order amount by customer type is $8.21 for business customers and $7.37 for regular customers.

---

## 📤 Outputs
- **Jupyter Notebook:** End-to-end analysis with visualizations and commentary  
- **`sku_summary.csv`:** SKU-level aggregated metrics for downstream use  
- Clear **Insights & Recommendations** section suitable for stakeholders  

---

## 🚀 How to Run
1. Clone the repository  
2. Place `amazon_sales.csv` in the project directory  
3. Open the notebook:
   ```bash
   jupyter notebook Amazon_Sales_Analysis.ipynb
