# Bank Customer Churn and Profitability Analytics

## Overview
This project analyzes retail banking customers to identify profitability drivers and churn risk using SQL and Power BI.

Using a normalized MySQL schema and rule-based churn scoring, the dashboard highlights high-value customers at risk of attrition and provides insights to support retention strategies.

## Tools Used
- MySQL 8.0
- Power BI Desktop
- SQL (CTEs, views, joins)
- DAX (measures and calculated columns)

## Data
- Public bank churn dataset (Kaggle: Churn Modelling)
- 10,000 customer records across demographics, products, balances, and churn outcomes

## Data Model
- Staging table for raw churn data
- Dimension tables for customers and geography
- SQL views for:
  - customer profiles
  - profitability estimation
  - churn risk scoring
  - high-value at-risk customers

## Key Metrics
- Annual customer profit (fee + balance-based proxy – servicing cost)
- Churn rate
- Rule-based churn risk score
- Profitability segments

## Dashboards
### Executive Overview
![Executive Overview](screenshots/Executive_Overview.png)

### Profitability and Segmentation
![Segmentation](screenshots/Profitability_and_Segmentation.png)

### Churn Risk and Retention Actions
![Churn Risk](screenshots/Churn_Risk_and_Retention_Actions.png)

## Key Insights
- Medium and high profit customers contribute the majority of total profit
- Churn risk increases significantly among low-profit and single-product customers
- A subset of high-profit customers exhibit elevated churn risk and should be prioritized for retention outreach

## Assumptions
- Profitability is estimated using simplified fee and balance-based revenue proxies
- Churn risk is rule-based for explainability
- Dataset churn labels are treated as historical outcomes

## Next Steps
- Add transaction-level data for behavioral churn signals
- Incorporate predictive churn modeling
- Simulate retention interventions and ROI
