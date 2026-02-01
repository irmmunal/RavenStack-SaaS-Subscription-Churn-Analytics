# RavenStack SaaS Churn Analysis

A comprehensive data analysis project investigating customer retention patterns and identifying critical business issues for a B2B SaaS company.

---

## Dataset Credit

**Original Dataset:** RavenStack Synthetic SaaS Dataset (Multi-Table)  
**Author:** River @ Rivalytics  
**Source:** [Rivalytics Medium Blog]([https://rivalytics.medium.com](https://www.kaggle.com/datasets/rivalytics/saas-subscription-and-churn-analytics-dataset))  
**License:** MIT-like (fully synthetic, no PII)

*This analysis is built upon the RavenStack synthetic dataset created by River @ Rivalytics. All credit for the original data generation goes to the dataset author.*

---

## Overview

This project analyzes 500 customer accounts across 2023-2024 to understand churn patterns and provide actionable recommendations. The analysis uncovered a severe retention crisis that worsened throughout 2024.

**Dataset Details:**
- **accounts:** 500 rows
- **subscriptions:** 5,000 rows
- **feature_usage:** 25,000 rows
- **support_tickets:** 2,000 rows
- **churn_events:** 600 rows

---

## Key Findings

- **Churn increased 3x:** From 8% (Jan 2024) to 23% (Dec 2024)
- **Q4 2024 collapse:** 75% of December customers left in first month
- **Onboarding failure:** New customer segment shows 38% churn
- **Feature usage paradox:** High engagement doesn't prevent churn

**Bottom line:** RavenStack faces company survival risk without immediate intervention.

---

## Technologies Used

- **Python 3.x**
- **pandas** - Data manipulation and analysis
- **matplotlib** - Data visualization
- **seaborn** - Statistical visualizations
- **numpy** - Numerical operations
- **Jupyter Notebook** - Interactive analysis

---

## Project Structure
```
ravenstack-analysis/
│
├── data/
│   ├── ravenstack_accounts.csv
│   ├── ravenstack_subscriptions.csv
│   ├── ravenstack_feature_usage.csv
│   ├── ravenstack_support_tickets.csv
│   └── ravenstack_churn_events.csv
│
├── notebooks/
│   ├── 1_data_loading.ipynb
│   ├── 2_basic_metrics.ipynb
│   ├── 3_visualizations.ipynb
│   ├── 4_time_series_analysis.ipynb
│   ├── 5_feature_usage_analysis.ipynb
│   ├── 6_rfm_segmentation.ipynb
│   └── 7_cohort_analysis.ipynb
│
├── outputs/
│   ├── graphs/
│   └── reports/
│
├── EXECUTIVE_SUMMARY.md
└── README.md
```

---

## Analyses Conducted

### 1. Time Series Analysis
Tracked monthly churn rates to identify trend deterioration throughout 2024.

### 2. Feature Usage Analysis
Examined relationship between product engagement and retention (counter-intuitive findings).

### 3. RFM Segmentation
Segmented customers by Recency, Frequency, and Monetary value to identify at-risk groups.

### 4. Cohort Analysis
Compared retention rates across signup cohorts to reveal Q4 2024 collapse.

### 5. Industry & Plan Tier Analysis
Identified DevTools segment as highest risk (31% churn).

### 6. Billing Frequency Analysis
Tested hypothesis that contract type affects retention (minimal impact found).

---

## How to Run

### Prerequisites
```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### Run Analysis
```bash
jupyter notebook
```

Open notebooks in sequence (1-7) to reproduce analysis.

---

## Key Insights for Data Analysts

### What Worked
- **Normalized metrics:** Used churn rate instead of absolute numbers
- **Cross-validation:** Multiple analyses confirmed same findings
- **Hypothesis testing:** Tested and disproved billing frequency assumption
- **Time-based analysis:** Revealed deterioration pattern invisible in aggregate data

### Unexpected Findings
- High engagement (feature usage) didn't prevent churn
- Best customers (Champions) also leaving despite satisfaction
- Contract type (monthly vs annual) had no impact on retention
- Big spenders most stable despite low usage

---

## Business Recommendations

**Immediate:**
1. Pause customer acquisition
2. Emergency product audit (Q4 changes)
3. Fix onboarding experience

**Short-term:**
4. Expand customer success team
5. Focus on DevTools segment
6. Interview churned Champions

See [EXECUTIVE_SUMMARY.md](EXECUTIVE_SUMMARY.md) for detailed recommendations.

---

## Skills Demonstrated

- Data cleaning and quality control
- Exploratory data analysis (EDA)
- Time series analysis
- Customer segmentation (RFM)
- Cohort retention analysis
- Statistical hypothesis testing
- Data visualization
- Business insight translation

---

## License

This analysis is built on the RavenStack synthetic dataset by River @ Rivalytics, distributed under MIT-like license. The analysis code and insights are original work by Irem Unal.

---

## Acknowledgments

- **Dataset:** RavenStack Synthetic SaaS Dataset by River @ Rivalytics
- **Analysis Framework:** Inspired by SaaS retention best practices and industry benchmarks

---

*Note: This is a portfolio project using synthetic data for demonstration purposes. All findings and recommendations are based on simulated scenarios.*
