# Pharmaceutical Sales & Demand Seasonality Analysis

## 📌 Project Overview
This project delivers an end-to-end Exploratory Data Analysis (EDA) on multi-year pharmaceutical sales transactions across 8 therapeutic drug classes (ATC classifications). The goal is to analyze historical volume trajectories, assess product portfolio concentration, uncover seasonal demand fluctuations, and provide actionable inventory procurement guidelines.

---

## 🛠️ Tools & Techniques
- **Tool:** Google Sheets / Advanced Spreadsheet Modeling
- **Techniques:** Data Cleaning & Parsing, Multi-dimensional Pivot Tables, Custom Date Grouping, Trend Analysis, Seasonality Indexing, Portfolio Pareto Analysis, Executive KPI Dashboarding.

---

## 📊 Key Insights & Findings

### 1. Portfolio Concentration (Pareto Principle)
- **Primary Driver:** Category **`N02BE`** (Analgesics/Antipyretics) accounts for **49.4%** (~62.5k units) of total pharmacy sales.
- **Secondary Baseline:** Category **`N05B`** (Psycholeptics) contributes **14.5%** (~18.3k units).
- **Long-tail Categories:** Categories such as **`N05C`** represent niche volume (~1.0%), highlighting extreme product concentration.

### 2. Time-Series Trends & Seasonality Cycles
- **Late Autumn / Winter Surge:** `N02BE` and `R03` (Respiratory) exhibit sharp demand acceleration starting in September/October and continuing through winter.
- **Spring Allergy Cycle:** Category `R06` (Antihistamines) displays a distinct demand peak in **April–May**.
- **Steady Baseline Categories:** `M01AB` (Anti-inflammatory) and `N05B` maintain non-cyclical, stable month-over-month consumption patterns.

---

## 📈 Dashboard Preview
![Dashboard Preview](docs/dashboard_overview.png)

---

## 💡 Business Recommendations
1. **Dynamic Safety Stock Sizing:** Initiate seasonal inventory buildup for `N02BE` and `R03` starting in August to mitigate severe Q4 stockout risks.
2. **Allergy Season Pre-ordering:** Adjust procurement lead times for `R06` ahead of Q2 to meet recurring spring demand surges.
3. **Working Capital Optimization:** Maintain lean safety stock during low-demand summer periods (June–July) to minimize inventory holding costs.

---

## 📁 Repository Structure
- `data/`: Raw transaction dataset (`salesmonthly.csv`).
- `docs/`: Visual assets and dashboard screenshots.
- `README.md`: Project summary, methodology, and strategic takeaways.
