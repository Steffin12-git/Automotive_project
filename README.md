# AtliQ Motors - India Market Entry Strategy

## 📄 Project Summary

This project, undertaken as a data analyst for AtliQ Motors India, focuses on a detailed market study of the Indian electric and hybrid vehicle sector. The goal is to provide data-driven insights and strategic recommendations to the Chief of AtliQ Motors India, Bruce Haryali, to inform the company's expansion plans.

---

## ❓ Problem Statement

AtliQ Motors, an automotive giant from the USA, is planning to launch its best-selling electric and hybrid vehicles in India. Currently, their market share in India is less than 2%. The task is to analyze the existing EV/Hybrid market in India, answer a set of primary and secondary research questions, and present the findings in a clear, self-explanatory dashboard to support the decision-making process.

---

## 📊 Data Sources

The analysis is based on the following datasets:

* **electric\_vehicle\_sales\_by\_state.csv**: Monthly sales data for electric and total vehicles across various states and vehicle categories (2-Wheeler, 4-Wheeler).
* **electric\_vehicle\_sales\_by\_makers.csv**: Monthly sales data for electric vehicles by individual manufacturers and vehicle categories.
* **dim\_date.csv**: A date dimension table to facilitate time-series analysis and filter data by fiscal year and quarter.
* **meta\_data.txt**: Key definitions for metrics like Penetration Rate and Compound Annual Growth Rate (CAGR).

---

## 📌 Key Metrics and DAX Measures

Several custom DAX measures were created to address the business questions, including:

* **Penetration Rate**: Calculates the proportion of electric vehicles sold relative to the total vehicle sales.
* **CAGR (Compound Annual Growth Rate)**: Computes the yearly growth rate in EV and total vehicle sales between 2022 and 2024.
* **Revenue Growth Rate**: Estimates revenue growth using average unit prices of EVs.
* **Top N/Bottom N Ranking Filters**: Used to dynamically filter states or makers based on top or bottom N performance in penetration or sales.
* **Forecasting Future Sales**: Projects sales for 2030 using CAGR assumptions.

---

## 📈 Primary Research Questions & Power BI Solutions

* **Top/Bottom Makers**: Used RANKX and slicers for Top N/Bottom N logic on 2W sales for FY2023 and FY2024.
* **Top States by EV Penetration**: Calculated penetration and used dynamic slicers for Top N (3,5,10, etc.).
* **States with Declining Penetration**: Created a measure comparing 2022 vs 2024 penetration and filtered for decline.
* **Quarterly Trends (Top 5 Makers)**: Merged date table with sales data; used Quarter on X-axis.
* **Delhi vs Karnataka EV Sales**: Used Card visuals and Clustered Bar charts for EV Sales and Penetration.
* **CAGR Top 5 Makers**: Calculated CAGR using DAX; applied slicers for 4W and fiscal years.
* **Top 10 States by CAGR (All Sales)**: Ranked by CAGR on total vehicle sales.
* **Seasonal Trends**: Extracted short month names and plotted sales using a line/column chart.
* **2030 EV Projections**: Used CAGR to forecast sales.
* **Revenue Analysis**: Estimated revenue using average prices and sales figures.

---

## 📚 Secondary Research Questions & Insights

* **Customer Preferences**: Cost savings, environmental impact, tax benefits, and smart features.
* **Govt Incentives**: Higher for 4W (FAME-II, Section 80EEB) vs 2W.
* **Charging Infra Correlation**: States with strong infra (Delhi, KA, MH) show higher penetration.
* **Brand Ambassador**: Recommended **Ranveer Singh** for mass appeal and tech image.
* **Ideal State for Manufacturing**: Tamil Nadu — due to policy, infra, skilled labor, and stability.

---

## 🚀 Top 3 Strategic Recommendations

1. **Launch Strategy**: Use a dual EV/Hybrid launch model + Brand ambassador for reach.
2. **Manufacturing + Infra**: Set up unit in TN + Charging infra across target markets.
3. **Product & Support**: Deliver high-quality vehicles with strong after-sales and support.

---

## 🧰 Tools Used

* Microsoft Power BI
* Power Query
* DAX (Advanced Level)
* Excel for initial data validation
* Government reports & market insights for secondary research
