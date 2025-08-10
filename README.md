# E-Commerce Customer Behavior Analytics Dashboard

This project analyzes real-world e-commerce transaction data to understand customer behavior, retention patterns, and promotional impact using SQL, Python, and data visualization techniques.

## Project Overview

The dataset contains transaction records from a UK-based online retail store. The analysis focuses on customer lifecycle behavior, including first purchase timing, repeat behavior, and long-term retention.

## Data Cleaning and Transformation

Raw transaction data was cleaned using SQL and Python. Invalid dates, missing CustomerIDs, and formatting issues were resolved. Key fields such as OrderMonth and OrderDayOfWeek were derived to support time-based analysis.

## RFM Analysis (Recency, Frequency, Monetary)

Customers were scored and segmented based on:
- Recency: How recently they made a purchase  
- Frequency: How often they purchased  
- Monetary: How much they spent  

Segments included Champions, Loyal Customers, At Risk, and Churned customers. This helped identify high-value customers and prioritize retention strategies.

## Cohort Analysis

Customers were grouped by their first purchase month (CohortMonth). Retention was measured over time to evaluate long-term engagement.

From cohort_retention_percent.csv (Retention %):
- 2010-01 Cohort:
  - Month 0: 100.0%
  - Month 12: 15.4%
  - Month 24: 10.7%
  - Month 36: 14.1%
  - Month 48: 12.0%
  - Month 60: 14.1%
  - Month 72: 14.9%
  - Month 84: 13.6%

From cohort_analysis.csv (Customer Counts):
- 2010-01 Cohort:
  - Month 0: 383 customers
  - Month 12: 59
  - Month 24: 41
  - Month 36: 54
  - Month 48: 46
  - Month 60: 54
  - Month 72: 57
  - Month 84: 52

Insight: While most customers drop off within the first few years, a small but consistent group remains active even after 7+ years, indicating long-term customer loyalty and opportunities for re-engagement.

## A/B Test Simulation

Customers were randomly assigned to two groups:
- Group A: Received a simulated promotional offer  
- Group B: No promotion  

Average spending was compared using a t-test.  
Result: p-value = 0.792  
Conclusion: No statistically significant difference in spending between groups. The promotional campaign did not have a measurable impact.

## Key Takeaways

- Customer retention drops sharply after the first year  
- A small cohort of customers remains active for over 7 years  
- High-value segments can be identified using RFM scoring  
- Statistical testing supports data-driven decision-making  

This project demonstrates end-to-end analytical skills—from data cleaning to insight generation—using real-world e-commerce data.