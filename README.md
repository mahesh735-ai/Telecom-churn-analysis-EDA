# 📉 Telecom Customer Churn Analysis — EDA Project

> **"1 in 4 customers is about to leave. This project finds out why."**

---

## 🧠 Problem Statement

Customer churn is one of the most critical challenges in the telecom industry. When a customer cancels their subscription and migrates to a competitor, it directly erodes **Monthly Recurring Revenue (MRR)**. This project performs a deep Exploratory Data Analysis (EDA) to uncover *why* customers churn — and which segments are most at risk — so targeted retention strategies can be deployed instead of costly generic discounts.

---

## 📂 Dataset

| Attribute | Detail |
|-----------|--------|
| **Source** | [Kaggle — Telco Customer Churn (IBM Sample Dataset)](https://www.kaggle.com/datasets/blastchar/telco-customer-churn) |
| **Records** | 7,043 customers |
| **Features** | 21 (demographic, service, billing, churn label) |
| **Target Variable** | `Churn` (Yes / No) |
| **Overall Churn Rate** | **26.5%** |

---

## 🔍 Key Findings

### 🚨 The Danger Window
Churn **peaks violently within the first 0–5 months** of a customer's tenure. Customers who survive past 20 months show significantly higher loyalty.

| Tenure Group | Churn Rate |
|---|---|
| < 1 Year | ~50% |
| 1–3 Years | ~35% |
| 3+ Years | ~15% |

---

### 📄 Contract Type — Biggest Differentiator
Month-to-month customers churn at **14× the rate** of two-year contract customers.

| Contract | Churn Rate |
|---|---|
| Month-to-Month | 42% |
| One-Year | 11% |
| Two-Year | 3% |

---

### 💳 Payment Method — The Electronic Check Problem
Customers using electronic checks churn at **3× the rate** of credit card users.

| Payment Method | Churn Rate |
|---|---|
| Electronic Check | ~45% |
| Mailed Check | ~19% |
| Bank Transfer (Auto) | ~17% |
| Credit Card (Auto) | ~15% |

---

### 🌐 Internet Service — The Fiber Paradox
Despite being the premium tier, **Fiber Optic users churn more than DSL users** — particularly those without Tech Support or Online Security (the "Ecosystem Deficit").

| Internet Service | Churn Rate |
|---|---|
| Fiber Optic | ~30% |
| DSL | ~20% |
| No Internet | ~7% |

---

### 👴 Senior Citizens — High-Risk Demographic
Senior citizens (65+) churn at nearly **double the rate** of non-seniors.

| Segment | Churn Rate |
|---|---|
| Senior Citizens | ~41.7% |
| Non-Senior Citizens | ~23.6% |

---

## 🛠 Tech Stack

| Tool | Purpose |
|------|---------|
| **Python 3** | Core language |
| **Pandas** | Data manipulation & cleaning |
| **NumPy** | Numerical operations |
| **Matplotlib** | Base visualizations |
| **Seaborn** | Statistical plots |
| **Google Colab** | Development environment |

---

## 📊 Analysis Performed

- ✅ Data loading & shape inspection
- ✅ Data type correction (`TotalCharges` blank → `0` → `float`)
- ✅ Null value & duplicate checks
- ✅ Univariate analysis (countplots, pie charts, histograms)
- ✅ Bivariate analysis (churn by contract, payment, tenure, service, demographics)
- ✅ Stacked percentage bar charts (crosstab normalization)
- ✅ Tenure distribution analysis by churn status

---

## 💡 Strategic Recommendations

1. **Promote Long-Term Contracts** — Incentivize month-to-month users to switch to annual plans
2. **Fix the Electronic Check Problem** — Campaign to migrate users to auto-pay methods
3. **Aggressive Early-Tenure Onboarding** — 90-day structured engagement for new customers
4. **Fiber Optic Quality Audit** — Bundle Tech Support & Online Security with premium plans
5. **Senior Citizen Retention Program** — Dedicated support channels & tailored pricing

---

## 📁 Project Structure

```
📦 Telecom-Churn-Analysis
 ┣ 📓 Churn_analysis_EDA_P2.ipynb    ← Main analysis notebook
 ┣ 📊 Customer_Churn.csv              ← Dataset (Kaggle Telco)
 ┗ 📄 README.md                       ← This file
```

---

## 🚀 How to Run

```bash
# Clone or download the repository
# Open the notebook in Google Colab or Jupyter

# Install dependencies (if running locally)
pip install pandas numpy matplotlib seaborn

# Run all cells in Churn_analysis_EDA_P2.ipynb
```

---

## 🙋 Author

**Prathamesh Chaudhari**
Data Analytics Enthusiast | Python | EDA | Business Insights

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin)](www.linkedin.com/in/mahesh-thakare-75817b2a7)

---

*Dataset: Kaggle — Telco Customer Churn | Analysis: EDA Only | Tools: Python, Pandas, Seaborn*
