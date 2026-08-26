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
<img width="815" height="122" alt="Screenshot 2026-08-26 at 1 32 34 AM" src="https://github.com/user-attachments/assets/f946c63f-19c0-4bf6-9b13-d7e16a5bbd1c" />
<img width="817" height="253" alt="Screenshot 2026-08-26 at 1 32 44 AM" src="https://github.com/user-attachments/assets/0d84fcf8-37eb-42cb-a1e1-cd5be7afe6de" />
<img width="603" height="374" alt="Screenshot 2026-08-26 at 1 32 53 AM" src="https://github.com/user-attachments/assets/21175865-c61b-4685-a680-2dc3355abe94" />
<img width="709" height="239" alt="Screenshot 2026-08-26 at 1 33 00 AM" src="https://github.com/user-attachments/assets/1a08e149-4cab-4187-a34b-cc33ce910e14" />


---

## 💡 Business Recommendations
1. **Dynamic Safety Stock Sizing:** Initiate seasonal inventory buildup for `N02BE` and `R03` starting in August to mitigate severe Q4 stockout risks.
2. **Allergy Season Pre-ordering:** Adjust procurement lead times for `R06` ahead of Q2 to meet recurring spring demand surges.
3. **Working Capital Optimization:** Maintain lean safety stock during low-demand summer periods (June–July) to minimize inventory holding costs.

---

## 📈 Year-over-Year (YoY) Market Dynamics

* **Long-Term Growth Drivers**: Category **R03** (Respiratory) showed sustained multi-year volume expansion, growing **+116.5%** between 2014 (1,277 units) and 2018 (2,765 units). **R06** (Antihistamines) expanded steadily with an overall growth of **+44.5%**.
* **2017 Market-Wide Contraction**: Total sales volume dropped by **-35.3% YoY in 2017** across all eight therapeutic categories before recovering with a **+39.6% rebound in 2018**.
* **Pattern Consistency**: Seasonal peak periods (Q4 winter surge for analgesics/respiratory and Q2 spring surge for antihistamines) remained stable year-over-year regardless of macroeconomic volume shifts.

---

## 📋 Prioritized Decision Matrix

| Category | Volume Share (%) | Seasonality (CV %) | Peak Period | Demand Pattern | Business Priority | Recommended Operational Action |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **N02BE** | 49.4% | 25.0% | Oct–Dec | High-Volume Surge | **Tier 1 (Critical)** | Pre-season buffer build starting in Sep; dynamic reorder points |
| **N05B** | 14.5% | 7.7% | Stable | High-Volume Baseline | **Tier 2 (High)** | Continuous replenishment; fixed safety stock to control holding costs |
| **R03** | 9.3% | 27.9% | Dec–Jan | Winter Respiratory Spike | **Tier 2 (High)** | Procurement ramp in Q3; track supplier lead times ahead of winter |
| **R06** | 4.8% | 48.0% | Apr–May | Spring Allergy Surge | **Tier 2 (High Seasonality)** | Strategic Q1 pre-orders before April peak; summer destocking |
| **M01AB** | 8.3% | 8.2% | Stable | Steady Demand | **Tier 3 (Medium)** | Standard periodic inventory review; steady baseline sourcing |
| **M01AE / N02BA** | ~6.4% each | < 7.0% | Stable | Steady Demand | **Tier 3 (Medium)** | Standard periodic review; lean baseline inventory |
| **N05C** | 1.0% | 13.7% | Jan | Low-Volume Niche | **Tier 4 (Low)** | Lean min-max ordering to avoid product expiration |

---

## ⚠️ Limitations

* **Absence of Operational & Supply Data**: Actual warehouse inventory levels, replenishment cycle times, supplier lead times, and historical stockout logs were unavailable; recommendations serve as planning guidelines rather than calculated Economic Order Quantities ($EOQ$).
* **Unmodelled Demand Drivers**: The dataset reflects aggregate sales volumes without external covariates such as epidemiological trends (flu season severity), meteorological data, regulatory changes, or marketing/pricing promotions.
* **Correlation vs. Causality**: The analysis establishes recurring historical seasonality and volume trends but does not isolate causal drivers behind structural demand shocks (such as the 2017 volume drop).
* **Financial & Capital Quantification**: Quantifying exact carrying cost savings and stockout reduction percentages requires integration with unit pricing, COGS, and inventory holding cost ledgers.

## 📁 Repository Structure
- `data/`: Raw transaction dataset (`salesmonthly.csv`).
- `docs/`: Visual assets and dashboard screenshots.
- `README.md`: Project summary, methodology, and strategic takeaways.
