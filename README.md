# 💳 Customer Credit Risk Segmentation – Data Analysis Project

## 🧩 Business Context

A financial institution aims to enhance its credit risk management, loan approval decisions, and product personalization by analyzing client data. Currently, the bank lacks a systematic segmentation of clients based on risk or potential value, which leads to losses due to defaults and missed retention opportunities.

This project leverages a synthetic dataset enriched with demographic, behavioral, and financial variables to:

- Identify hidden patterns in customer behavior
- Group clients by risk and opportunity
- Enable better targeting of financial products

---

## 🎯 Project Objectives

- Analyze the demographic and financial characteristics of clients.
- Identify client segments using clustering techniques.
- Evaluate risk levels through combinations of credit score, loan behavior, and tenure.
- Understand which profiles are most likely to default or be approved for loans.
- Build a dashboard to assist risk and marketing teams in decision-making.

---

## 🧰 Tools Used

- **Excel** – Data simulation and transformation
- **Python (Jupyter Notebook)** – Data analysis and KMeans segmentation
- **Seaborn & Matplotlib** – Data visualization
- **Scikit-learn** – Clustering and preprocessing
- **Power BI** – Interactive dashboard
- **GitHub** – Project tracking and documentation

---

## 📊 Dataset Description

The dataset contains over 200 synthetic client records, with the following variables:

| Column               | Description                                  |
|----------------------|----------------------------------------------|
| `Age`                | Client's age                                 |
| `Gender`             | Male or Female                               |
| `Income`             | Annual income in USD                         |
| `Education`          | Education level                              |
| `Marital Status`     | Single or Married                            |
| `Number of Children` | Number of dependent children                 |
| `Home Ownership`     | Owned or Rented                              |
| `Credit Score`       | Low / Average / High                         |
| `Loan Approved`      | Whether the client received a loan approval  |
| `Defaulted`          | Whether the client defaulted on a loan       |
| `Customer Tenure`    | Years as a client                            |
| `Product Type`       | Type of product held (e.g., mortgage, card)  |
| `Risk Level`         | Derived risk classification (High/Medium/Low) |

---

## 🔍 Process Summary

1. **Data Exploration & Cleaning**
   - Null checks, types, and distributions
   - Initial univariate and bivariate analysis

2. **Feature Engineering**
   - Encoding `Credit Score` numerically
   - Creating `Risk Level` from behavior and score

3. **Clustering**
   - KMeans with `Age`and `Income`
   - Elbow Method to find optimal number of clusters
   - Levels of segmentation:
     - Simple (2D: Age vs Income)

4. **Visualization**
   - Distributions by risk
   - Cluster scatterplots
   - Cross-tabulations and statistical summaries

5. **Power BI Dashboard**
   - KPIs by segment
   - Loan approval and default rates
   - Risk level breakdown by tenure and score
   - Product type distribution by cluster

---

## 📈 Key Insights

- Clients with **Low Score + High Loan Amount** show the highest default probability.
- High-score clients with **long tenure** are consistently low risk.
- Product distribution suggests **Mortgage and Personal Loan** are concentrated in high-risk segments.
- Segment 0 (young + low income) is at higher risk and lower approval rate.

---

## 💼 Recommendations

- **Tighten approval policies** for clients with low credit score and income below $50,000.
- Design **preventive strategies** for new clients with short tenure and high loan amounts.
- Target **Segment 2** (older clients with high income and low risk) for cross-selling investments.
- Use `Customer Tenure` to guide loyalty programs.

---
