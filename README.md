# plant_sales_dashboard
Here is the complete project documentation and analysis for the **Plant Co. Gross Profit Performance** dashboard, structured according to the recommended framework in your guidelines:

---

## 1. Project Title / Headline

🌱 **Plant Co. Analytics: Gross Profit Performance & Profitability Segmentation Dashboard**

An interactive financial analytics dashboard designed to track Year-to-Date (YTD) gross profit performance against Prior Year-to-Date (PYTD), identify regional revenue leakages, and segment account profitability across product lines.

---

## 2. Short Description / Purpose

This dashboard provides executive leadership and financial analysts at Plant Co. with an end-to-end view of gross profit trends, sales quantities, and overall profitability. It exists to quickly diagnose the root causes of underperformance—specifically identifying which countries, months, and product categories (Indoor, Landscape, Outdoor) are driving year-over-year profit declines.

---

## 3. Tech Stack

The dashboard was built using the following business intelligence tools and techniques:

* **Power BI Desktop:** Main visualization and reporting engine used to design the interactive layout.
* **Power Query:** Data ingestion and cleaning layer used to model transaction history, accounts, and regional mapping.
* **DAX (Data Analysis Expressions):** Utilized for time-intelligence calculations (`YTD`, `PYTD`, `YTD vs PYTD`), dynamic metric switching (Gross Profit, Quantity, Sales), and custom segmentation logic.
* **Data Modeling:** Star-schema relational model linking sales transactions to product catalogs, geographical regions, and account profiles.

---

## 4. Data Source & Structure

* **Source:** Plant Co. Enterprise Resource Planning (ERP) and sales transaction databases.
* **Structure:** Contains multi-year transactional records aggregated by **Year** and **Month**, categorized by **Country** (global operations), **Product Type** (*Indoor*, *Landscape*, *Outdoor*), and individual client **Accounts**, tracking core financial metrics including Sales Volume, Quantity Sold, and Gross Profit Margins.

---

## 5. Features / Highlights

### **Business Problem**

Plant Co. is experiencing a severe downward trend in overall profitability, with current Year-to-Date Gross Profit falling significantly behind the previous year's performance (**-$5.49M** variance). Without granular visibility into regional and product-level dynamics, management cannot pinpoint where the greatest financial losses are occurring or which client accounts are underperforming.

### **Goal of the Dashboard**

* Quantify total YTD gross profit and margin percentage against historical baselines.
* Isolate the specific geographic regions and months contributing most to the profit deficit.
* Evaluate product mix performance across different seasons.
* Segment individual accounts by profit volume and gross margin percentage to optimize sales strategy.

### **Walkthrough of Key Visuals**

* **KPI Summary Cards:** Instantly display core high-level metrics—YTD Gross Profit (**1.40M**), Year-over-Year variance (**-5.49M**), PYTD baseline (**6.89M**), and overall Gross Profit Margin (**39.77%**).
* **Bottom 10 YTD vs PYTD | Country (Treemap):** Highlights the underperforming geographical markets. **China** is the single largest contributor to the deficit (**-$1.93M**), followed by **Brazil** (**-$0.38M**) and the **Philippines** (**-$0.31M**).
* **Gross Profit YTD vs PYTD (Waterfall Chart):** Breaks down the cumulative profit variance across countries and timeframes, allowing users to trace how specific market drops accumulate into the total -$5.49M loss.
* **Gross Profit YTD & PYTD | Month (Stacked Column & Line Chart):** Compares monthly YTD performance across product types (*Indoor*, *Landscape*, *Outdoor*) against the PYTD trendline. It reveals a massive performance drop during Q1 (January–March), where previous year values were between **$0.76M–$0.92M**, but current YTD values barely reach **$0.39M–$0.40M**.
* **Account Profitability Segmentation (Scatter Plot):** Maps individual accounts by **Value YTD** (X-axis) against **Gross Profit %** (Y-axis). Reference lines at **40% GP** and **~$8K Value YTD** divide clients into four distinct quadrants (e.g., high-volume/high-margin champions vs. low-margin/high-maintenance accounts).

### **Business Impact & Insights**

* **Geographical Interventions:** Management must urgently review operations and sales strategies in **China**, as it accounts for over **35% of the total global profit decline**.
* **Seasonal & Product Strategy:** The stark drop in Q1 performance indicates that winter/early-spring sales strategies for *Indoor* and *Landscape* plants failed to repeat last year's success. Promotional campaigns should be adjusted ahead of Q1 next year.
* **Account Optimization:** Sales teams can use the scatter plot segmentation to renegotiate pricing with high-volume accounts sitting below the **40% profit margin threshold**, while creating loyalty programs for accounts in the top-right quadrant.
