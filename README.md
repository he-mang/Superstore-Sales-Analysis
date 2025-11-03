# 📊 Superstore Sales Analysis (Excel)

**Author:** Hemang Chaudhary  
**Tools Used:** Microsoft Excel (PivotTables, Slicers, Conditional Formatting)  
**Dataset:** [Superstore Dataset – Kaggle](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)  

---

## 🧠 Project Overview
This project analyzes the **Superstore dataset** to uncover insights about sales performance, product profitability, discount impact, and customer behavior between **2014–2017**.  
The analysis was performed entirely in **Excel**, featuring **data cleaning**, **KPI calculations**, **PivotTable analysis**, and **interactive dashboards** with slicers for year-based filtering.

---

## 🎯 Objectives
The goal was to analyze sales, profit, and customer trends to identify:
- Which **regions, states, and categories** drive the most sales and profit  
- Which **products** are most and least profitable  
- How **discounts** affect profitability  
- Which **customer segments** bring the most revenue  
- How **sales and profit** evolve over time  

---

## 💡 Key Analytical Insight: Discount Profitability

The analysis revealed that discounts are the single largest driver of negative profit margin. The primary actionable insight is the clear threshold for when discounts transition from driving lower margin sales to causing significant losses.

| Discount Range | Total Profit | Profit Margin (%) |
|:---|:---|:---|
| 0% | **+\$320,987.60** | **29.51%** |
| 10% - 20% | **+\$10,448.17** | **12.75%** |
| 20% - 30% | **+\$90,337.31** | **11.82%** |
| **30% - 40%** | **-\$12,748.36** | **-10.86%** |
| **40% - 50%** | **-\$25,550.16** | **-20.96%** |
| **> 50%** | **-\$97,065.48** | **-78.82%** |

**Conclusion:** The Superstore must re-evaluate any discount policy that authorizes discounts **above 20%**, as these ranges are directly responsible for the majority of the company's losses.

---

## 🧹 Data Cleaning & Preparation
Steps performed in Excel:
1. **Converted dates** to proper Excel date format and extracted **Year, Month, and Day of Week**.  
2. Added helper columns:
   - `Profit Margin` = `Profit / Sales`
   - `Discount Range` using nested IF formulas  
   - `Shipping Days` = `Ship Date – Order Date`
   - `Distinct Customer Flag` (1 per unique customer per year)
3. Categorized discounts data into a discount range column for focused analysis.  
4. Removed blank or duplicate entries and standardized category and subcategory names.

---

## 📊 Business Questions and Analysis

## 🏷️ **Sales Analysis**
### 1. How have sales and profit trends evolved over time?
<img width="1051" height="277" alt="image" src="https://github.com/user-attachments/assets/4508551d-2a2c-4a7f-ae9e-8eb367228ee6" />

**Yearly Trend:** The business experienced strong overall growth from 2014 to 2017, with a major surge in 2016 and continued high growth in 2017.

### 2. Is there an overall growth or decline in sales and profit?
There is a clear overall positive growth in both total sales and total profit across the four years (2014 to 2017). The business is expanding. However, the search data suggests the overall Profit Margin is slightly declining in 2017 compared to 2016 (12.74% vs. 13.42%), indicating that costs or discounts are rising faster than sales prices.

### 3. Which periods experienced high or low sales and profit?
<img width="1361" height="609" alt="image" src="https://github.com/user-attachments/assets/5e88fe29-a931-4276-8590-0cef7fff1a28" />


**High Periods (Target):** Q4 (October, November, December), particularly November, which is the peak month for both sales and profit across all years.

**Low Periods (Avoid/Focus Improvement):** Q1 (January, February, March), with February typically being the lowest performing month.

### 4. What is the geographical distribution of sales and profit & which region generates the most sales?
<img width="1362" height="896" alt="image" src="https://github.com/user-attachments/assets/e59c1e3a-4ea2-4685-b4e7-9c51968d4fbb" />

**Top Region:** The West region generates the highest total sales and profit across all years.

**Geographical Concentration:** California and New York are the top two states contributing the highest total profit. Focus resources here to maintain market dominance.

### 5. What are the profit margin and loss (%) by the state?
<img width="1364" height="455" alt="image" src="https://github.com/user-attachments/assets/8e586167-887e-4d9e-9bee-373389581b32" />

**Top 5 Profit Margins (Target):** States with the highest margins (e.g., District of Columbia: 45.09%) should be analyzed to replicate their successful strategies (low discount, efficient shipping).

**Top Loss States (Avoid/Mitigate):** The states contributing the highest total losses are typically Texas, Pennsylvania, and Ohio. These states demand immediate review due to high discounts and/or high shipping costs.

## 📦 **Product Analysis**
### 6. What is the distribution of sales by product category & which category generates the highest revenue and profit?

**Highest Revenue and Profit:** Technology is the clear leader in both total sales and total profit.

**Highest Margins:** Technology and Office Supplies have very healthy and similar profit margins (over 17%).

**Lowest Margin (Avoid/Mitigate):** Furniture has high total sales but a severely low profit margin (<3%) across the 4 years, indicating significant issues with cost, discounts, or loss-making sub-categories.

### 7. What are the top-selling or most profitable products in the superstore?

**Top-Selling (by Sales Amount):** Canon imageCLASS 2200 Advanced Copier.

**Top-Profitable (by Profit):** Canon imageCLASS 2200 Advanced Copier. Other highly profitable sub-categories include Copiers, Phones, Accessories, and Paper.

**Loss-Making Products (Avoid/Mitigate):** The sub-category Tables consistently generates significant losses, making it a critical area to review (pricing, supplier costs, shipping, or discontinue low-profit items).

## 👥 **Customer Analysis**
### 8. Which customer segment generates the highest sales and profit?
<img width="859" height="603" alt="image" src="https://github.com/user-attachments/assets/9bb13dc6-400a-45de-87e8-e3e98c3eae26" />


**Highest Sales:** The Consumer segment generates the highest total sales.

**Highest Profit Margin (Target):** The Home Office and Corporate segments have a higher profit margin than the Consumer segment. This suggests that while Consumers buy more, Corporate and Home Office customers are more profitable per dollar of sale.

**Action:** Target the Corporate and Home Office segments for higher-margin products (e.g., Technology and Office Supplies).


All PivotTables are **linked to a Year slicer** for interactive filtering.

Each dashboard is dynamic, using slicer for **Year** filter, with unified fonts and color themes.

---

## 📏 Key Metrics & KPIs
| Metric | Description |
|--------|--------------|
| **Total Sales** | Overall revenue |
| **Total Profit** | Total profit earned |
| **Profit Margin** | Profit as % of sales |
| **Average Order Value (AOV)** | Sales per order |
| **Distinct Customers (per Year)** | Unique customers by year |
| **Top 3 Customers Leaderboard** | Top 3 customers by year with the largest sales amount |

---

## 🪄 Tools & Skills Demonstrated

1. Excel Data Cleaning
2. Data Modeling with Helper Columns
3. Pivot Tables & Charts
4. Slicers and Interactive Dashboards
5. Conditional Formatting for Profit/Loss Visualization
6. Analytical Storytelling through Dashboards

---

## 📬 Contact
**Author:** Hemang Chaudhary

**[LinkedIn](https://www.linkedin.com/in/hemangchaudhary)**
