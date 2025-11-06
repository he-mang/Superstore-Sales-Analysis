# 📊 APEX SUPPLIES: The Profit Erosion Crisis & The 20% Solution (2014-2017)

**A Data Analysis Project by:** Hemang Chaudhary  
**Tools Used:** Microsoft Excel (Advanced Formulas, PivotTables, Slicers, Conditional Formatting)
**Dataset:** [Fictional Apex Supplies Dataset – Kaggle](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)  

---

## 🧠 The Story: Growth on the Surface, Bleeding Beneath
Apex Supplies was facing a quiet crisis: top-line revenue looked strong with **20.36% YoY growth**, but the profit margin was shrinking. The question from leadership was simple: **"Where is our profit going?"**
<img width="720" height="720" alt="image" src="https://github.com/user-attachments/assets/4508551d-2a2c-4a7f-ae9e-8eb367228ee6" />

This project moved beyond simple reporting to isolate the hidden financial drain. By analyzing over 9,000 transactions, the data revealed that Apex was engaged in **profit-destroying behavior**—specifically, an unchecked discounting culture—that was actively masking its true operational profitability.

## 💡 The Key Discovery: The 30% Profit Tipping Point
The primary objective was to find the financial breaking point. Through custom data engineering, the analysis established a critical, data-backed threshold: any discount beyond 30% consistently moves the transaction from driving margin to incurring devastating losses.

This discovery exposed the hidden $135K cumulative loss.
| Discount Range | Total Profit | Profit Margin (%) |
|:---|:---|:---|
| 0% | **+\$320,987.60** | **29.51%** |
| 10% - 20% | **+\$10,448.17** | **12.75%** |
| 20% - 30% | **+\$90,337.31** | **11.82%** |
| **30% - 40%** | **-\$12,748.36** | **-10.86%** |
| **40% - 50%** | **-\$25,550.16** | **-20.96%** |
| **> 50%** | **-\$97,065.48** | **-78.82%** |

**Conclusion (The Actionable Mandate):** The indiscriminate discounting policy must be immediately halted. This strategy has cost Apex a cumulative $135,000 in losses (2014-2017). Enforcing a hard stop at the 20% discount mark is the fastest path to margin recovery and requires policy change, not just sales growth.

## 🛠️ The Solution: Data Engineering & Dashboarding
Solving this crisis required transforming the raw transactional data into actionable financial intelligence.

- **Custom Feature Engineering:** The most critical step was using nested IF formulas in Excel to create the Discount Range variable, which was not available in the raw data. This simple transformation unlocked the entire profitability analysis.
- **Flagging the Financial Health:** Calculated `Profit Margin %` and `YoY Variance` to expose the 0.68% **margin decline** in 2017 despite high sales, giving leadership a critical financial alert.
- **Dynamic Reporting:** Built a** C-level interactive dashboard** using **PivotTables, Slicers, and Conditional Formatting** to allow managers to instantly filter performance by Year, Region, and Product Category, replacing static reports with dynamic analysis.

## 🗺️ Beyond Discounts: Strategic Growth Pathways
The analysis also provided high-leverage insights to maximize profitable growth once the discounting issue is fixed:

### Geographical Strategy (Where to Win):
- **Profit Engines:** Confirmed the **West region** and states like **California** and **New York** are the company's highest profit generators. Resources must be poured into maintaining market dominance here.
- **Loss Mitigation:** Isolated **Texas, Pennsylvania, and Ohio** as the **highest loss-contributing states**. This mandates immediate audit to determine if the losses are due to excess discounting, high shipping costs, or unfavorable local competition.

### Product Portfolio Strategy (What to Sell):
- **The Crown Jewel:** The **Technology** category is Apex's highest revenue and profit driver, with its best-selling product, the **Canon Copier**, serving as the benchmark for high-margin pricing.
- **The Cost Center:** The **Furniture** category is confirmed as a major drag on margin, particularly the **Tables** sub-category, which is chronically loss-making. This segment should be the target for either extreme cost reduction or discontinuation.

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

### 9. What are the patterns, frequency, and volume of orders?
<img width="1250" height="619" alt="image" src="https://github.com/user-attachments/assets/09083afe-0854-4718-b221-6c3b61a5bc0a" />

Orders consistently rise throughout the year, peaking in November/December and dropping in January/February.

### 10. What is the average shipping time for each ship mode?

The different shipping modes (Standard Class, Second Class, First Class, Same Day) have different average shipping times.

Standard Class is typically the slowest, and Same Day is the fastest.

### 11. How are discounts distributed and what is the impact of discounts on sales?

The discount distribution shows that the majority of discounted items are discounted at 20%. However, a small number of orders receive very large discounts (up to 80%), which are typically the transactions that result in the largest losses.

The data shows that high discounts (specifically those greater than 40%) often lead to negative profits/losses.

Discounts are concentrated in certain low-profit sub-categories like Tables and Bookcases (often in the 40-80% range in high-loss states like Texas and Illinois).

---

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
