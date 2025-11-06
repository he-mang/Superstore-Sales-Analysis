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

   <img width="480" height="178" alt="image" src="https://github.com/user-attachments/assets/60d57259-5fac-4ee5-8ebe-ec7fde002720" />

- **Dynamic Reporting:** Built a **C-level interactive dashboard** using **PivotTables, Slicers, and Conditional Formatting** to allow managers to instantly filter performance by Year, Region, and Product Category, replacing static reports with dynamic analysis.

## 🗺️ Beyond Discounts: Strategic Growth Pathways
The analysis also provided high-leverage insights to maximize profitable growth once the discounting issue is fixed:

### Geographical Strategy (Where to Win):
- **Profit Engines:** Confirmed the **West region** and states like **California** and **New York** are the company's highest profit generators. Resources must be poured into maintaining market dominance here.

   <img width="720" height="720" alt="image" src="https://github.com/user-attachments/assets/e59c1e3a-4ea2-4685-b4e7-9c51968d4fbb" />

- **Loss Mitigation:** Isolated **Texas, Pennsylvania, and Ohio** as the **highest loss-contributing states**. This mandates immediate audit to determine if the losses are due to excess discounting, high shipping costs, or unfavorable local competition.

   <img width="480" height="360" alt="image" src="https://github.com/user-attachments/assets/6d6b93f0-06e2-4bcc-8066-8b9d4e42be3a" />


### Product Portfolio Strategy (What to Sell):
- **The Crown Jewel:** The **Technology** category is Apex's highest revenue and profit driver, with its best-selling product, the **Canon Copier**, serving as the benchmark for high-margin pricing.

    <img width="720" height="760" alt="image" src="https://github.com/user-attachments/assets/2b4f57c3-b207-4fc5-9924-cc05a752c34c" />

- **The Cost Center:** The **Furniture** category is confirmed as a major drag on margin, particularly the **Tables** sub-category, which is chronically loss-making. This segment should be the target for either extreme cost reduction or discontinuation.

     <img width="720" height="1080" alt="image" src="https://github.com/user-attachments/assets/c2d454e2-1a08-47c9-9cb0-95757b7e140a" />

**This project delivered not just data, but a clear, evidence-based mandate for pricing reform and strategic resource allocation across Apex Supplies' entire organization.**

---

## 📬 Contact
**Author:** Hemang Chaudhary

**[LinkedIn](https://www.linkedin.com/in/hemangchaudhary)**
