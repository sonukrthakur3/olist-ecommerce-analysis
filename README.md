# Olist E-Commerce: Marketplace Performance & Customer Experience Analysis

**Prepared by:** Sonu Kumar Thakur  
**Event:** Gradient Learnings Data Analytics Hackathon  

---

## Executive Summary
This project analyzes operational data spanning ~100,000 orders from Olist E-Commerce (Brazil) to identify drivers of customer satisfaction. Through data cleaning, metric engineering, and exploratory data analysis, the analysis isolates logistics bottlenecks, regional discrepancies ("Logistics Tax"), and category-specific fulfillment failures.

---

## Key Insights & Findings
1. **Quality vs. Growth Trade-off:** Peak demand events (e.g., Black Friday 2017) caused review scores to drop to 3.96 due to logistics strain.
2. **The "Delivery Cliff":** Delivery timing relative to SLA is the strongest driver of review ratings. On-time orders average 4.28 stars, dropping to 2.70 for 1–7 days late, and 1.69 for >7 days late.
3. **Geographic Asymmetry:** Concentration of sellers in the Southeast (São Paulo) creates high freight costs and >21-day delivery delays for North/Northeast buyers.
4. **Category Discrepancies:** Lightweight items (Toys, Health & Beauty) achieve ~4.22 stars, while bulky items (Furniture, Bed/Bath/Table) consistently underperform.
5. **Payment Friction:** Cash-based Boleto payments add multi-day clearing delays, pushing back seller dispatch triggers.

---

## Visualizations
![Monthly Trend](assets/chart1.png)
![Delivery Timing Impact](assets/chart2.png)
![Geographic Inequality](assets/chart3.png)

---

## Actionable Recommendations
1. **Dynamic SLA Buffering:** Implement data-driven delivery buffers for distant origin-destination pairs.
2. **Seller Dispatch Enforcement:** Enforce strict 48-hour seller dispatch policies with penalties/incentives.
3. **Regional Fulfillment Micro-Hubs:** Establish hubs in the Northeast to reduce freight costs and transit times.
4. **Specialized Freight Routing:** Partner with specialized carriers for heavy/bulky categories.
5. **Payment Expectation Messaging:** Clarify post-payment dispatch timelines at checkout for Boleto transactions.

---

## Tech Stack & Data Pipelines
- **Language:** Python 3
- **Libraries:** Pandas, Matplotlib, Seaborn
- **Environment:** Google Colab / Jupyter Notebook
