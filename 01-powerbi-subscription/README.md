# Project 01 — E-commerce Subscription Analytics

**Stack:** Python · scikit-learn · Prophet · Power BI · DAX · SQL

---

## Business Context

A subscription-based e-commerce company needed visibility into customer churn drivers,
revenue trends, and risk segmentation to support retention and growth strategies.
This project delivers an end-to-end analytics solution — from raw data to a Power BI
executive dashboard with an embedded machine learning churn prediction model.

---

## Dataset

- **Source:** IBM Telco Customer Churn (Kaggle)
- **Size:** 7,043 customers · 21 features
- **Domain:** Subscription services — monthly/annual contracts, recurring billing

---

## What Was Built

### 1. Exploratory Data Analysis
- Data quality assessment and cleaning
- Churn distribution across contract type, tenure, payment method and internet service
- Key finding: month-to-month contracts churn at 3x the rate of two-year contracts

### 2. Churn Prediction Model
- Logistic Regression and Random Forest classifiers
- Best model: Logistic Regression with AUC-ROC of 0.83
- Output: churn probability score per customer + risk segmentation (Low / Medium / High)

### 3. Revenue Forecasting
- Time series forecasting using Facebook Prophet
- 12-month revenue projection with confidence intervals
- Average forecasted monthly revenue: USD 10,443

### 4. Power BI Dashboard
- Real-time KPI cards: Churn Rate, MRR, Average Tenure, High Risk Customers
- Churn breakdown by contract, tenure group, payment method and internet service
- ML churn risk segmentation embedded from Python output
- Revenue forecast trend with confidence band

---

## Key Business Metrics

| Metric | Value |
|---|---|
| Total customers | 7,032 |
| Churn rate | 26.6% |
| High risk customers | 1,681 |
| Avg monthly charges | USD 64.80 |
| Model AUC-ROC | 0.83 |
| Forecasted avg MRR | USD 10,443 |

---

## Files

| File | Description |
|---|---|
| `01_exploratory_analysis.ipynb` | Full Python notebook — EDA, ML model, forecasting |
| `subscription_analytics.xlsx` | Cleaned dataset with churn probability scores |
| `revenue_forecast.xlsx` | 12-month revenue forecast data |
| `churn_analysis.png` | Churn distribution charts |
| `feature_importance.png` | ML feature importance chart |
| `revenue_forecast.png` | Revenue forecast visualization |
| `WA_Fn-UseC_-Telco-Customer-Churn.csv` | Raw dataset |
