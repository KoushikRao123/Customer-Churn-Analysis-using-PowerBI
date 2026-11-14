# Customer-Churn-Analysis-using-PowerBI
# 📊 Telco Customer Churn Analysis & Predictive Intelligence Dashboard

An end-to-end data analytics and predictive intelligence solution built to analyze customer attrition, uncover core behavioral and financial churn drivers, and empower telecommunications executives with actionable retention strategies.

---

## 🚀 Project Overview
Customer churn is one of the most critical business challenges in the telecommunications industry. This project transforms raw customer data into an interactive, multi-page Power BI dashboard designed to shift management from **reactive firefighting to proactive customer retention**.

---

## 🛠️ Tech Stack & Tools
* **Data Visualization & Dashboarding:** Microsoft Power BI (Service & Desktop)
* **Data Transformation & Modeling:** DAX (Data Analysis Expressions), Power Query
* **Programming & EDA Support:** Python (Pandas, Matplotlib, Seaborn)
* **Version Control:** Git & GitHub

---

## 📑 Dashboard Structure & Architecture

The solution is structured across **4 dedicated analytical pages** to provide a complete diagnostic and predictive narrative:

### 1. Customer Demographics Analysis
* **Core Focus:** Evaluates demographic splits (Gender, Senior Citizen status) and tenure patterns.
* **Key Visuals:** Donut charts for gender parity, area charts for tenure distribution, ribbon charts for monthly charge trends across tenure brackets, and executive KPI summary cards.

### 2. Service Subscriptions
* **Core Focus:** Analyzes the impact of core telecommunication services and digital add-ons on customer loyalty.
* **Key Visuals:** 100% stacked bar charts comparing internet types (DSL vs. Fiber Optic), AI-driven decomposition trees, multi-row KPI cards, and custom add-on usage metrics.

### 3. Contract & Billing Insights
* **Core Focus:** Examines financial structures, payment methods, and contract lengths.
* **Key Visuals:** Ribbon charts showing churn rate progression across contract tiers, waterfall charts tracking revenue impact, donut charts for payment friction analysis, and financial matrix tables.

### 4. Churn Prediction & Key Drivers
* **Core Focus:** Predictive risk modeling and root-cause identification.
* **Key Visuals:** Native AI **Key Influencers** visual, stacked area charts tracking retained vs. lost monthly recurring revenue (MRR), risk-tier distribution charts (High, Medium, Low Risk), and multi-level decision trees.

---

## 📐 Key DAX Measures & Logic
Core calculations implemented within the Power BI model include:
* **Total Customers:** `Total Customers = COUNTROWS('Telco Customer')`
* **Churned Customers:** `Churned Customers = CALCULATE([Total Customers], 'Telco Customer'[Churn] = "Yes")`
* **Churn Rate (%):** `Churn Rate = DIVIDE([Churned Customers], [Total Customers], 0)`
* **Tenure Group Categorization:** Custom `SWITCH` logic to segment customers into yearly cohorts (`0-1 Year`, `1-2 Years`, etc.).

---

## 💡 Strategic Business Recommendations
1. **Promote Long-Term Contracts:** Incentivize month-to-month customers (who experience ~40%+ churn) to migrate to annual agreements.
2. **Bundle Protective Add-ons:** Automatically bundle essential technical add-ons (Tech Support, Online Security) for Fiber Optic users to mitigate high early-stage drop-offs.
3. **First-Year Onboarding Interventions:** Deploy targeted engagement protocols during a customer's first 12 months, as attrition is heavily concentrated in the early tenure bracket.
4. **Automate Payment Methods:** Encourage users on manual electronic checks to transition to auto-pay bank transfers or credit cards to reduce billing friction.

---

## 📂 Repository Contents
* `Customer Churn Project.pbix` — The complete, interactive Power BI report file.
* `WA_Fn-UseC_-Telco-Customer-Churn.csv` — The underlying dataset used for analysis.
* `README.md` — Project documentation.

---
