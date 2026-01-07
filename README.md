# Customer-Segmentation-for-Financial-Services-using-Machine-Learning
End-to-end machine learning project that segments banking customers into actionable groups using behavioral, financial, and engagement data to drive marketing, risk, and revenue strategy.

# Project Summary
Built a finance-focused customer segmentation system using unsupervised learning (K-Means), advanced EDA, PCA visualization, KPI analysis, and business strategy mapping to support data-driven decision making in banking.

# Customer Segmentation for Financial Services

## Executive Summary
This project builds a machine learning–driven customer segmentation system for a financial institution. Using behavioral, financial, and engagement data, customers are grouped into actionable segments to improve revenue growth, cost optimization, and risk management.

## Business Objective
Segment customers into meaningful groups to:
- Increase marketing ROI  
- Improve cross-sell & upsell  
- Reduce servicing costs  
- Strengthen credit risk decisions  

## Dataset
Synthetic dataset of 1,500 banking customers containing:
Age, Income, CreditScore, AccountTenure, MonthlySpending, TransactionFrequency, AvgAccountBalance, NumProducts, AppUsageScore, SupportCalls.

## Methodology (CRISP-DM)

### 1. Business Understanding
Define segmentation use-cases for marketing, risk, and service strategy.

### 2. Data Understanding & EDA
Key findings:
- Income does not correlate strongly with savings.
- High support calls correlate with lower credit scores and balances.
- Young customers show high digital engagement but low balances.

### 3. Data Preparation
- Feature scaling
- Engineered metrics:
  - SpendingRatio = MonthlySpending / Income
  - EngagementScore = AppUsageScore * 2 - SupportCalls

### 4. Modeling
- Algorithm: K-Means Clustering
- Optimal clusters selected using Silhouette Score
- Final K = 4

### 5. Evaluation & Interpretation

| Segment | Persona | Key Characteristics |
|-------|--------|----------------|
0 | Premium Investors | High income, high balance, low risk |
1 | Lifestyle Spenders | High spending ratio, high transactions |
2 | Credit Dependent | Low income, low credit score, high support |
3 | Growth Segment | Young, digital-first, rising engagement |

### 6. PCA Visualization
Principal Component Analysis (2D) used for cluster visualization and validation.

## Business KPIs & Insights

### Estimated Customer Lifetime Value (CLV)
CLV proxy: AvgAccountBalance * AccountTenure / 10

| Segment | Estimated CLV | Risk Level | Digital Adoption |
|-------|--------------|-----------|----------------|
Premium Investors | Highest | Lowest | Medium |
Lifestyle Spenders | High | Medium | High |
Growth Segment | Medium | Low | Highest |
Credit Dependent | Lowest | Highest | Lowest |

### Strategic Impact

**Revenue Growth**
- Premium Investors → Wealth & investment products
- Lifestyle Spenders → Credit cards, EMI & rewards
- Growth Segment → Student loans, starter investments

**Cost Optimization**
- Reduce support cost by migrating Credit Dependent customers to digital self-service

**Risk Management**
- Credit Dependent cluster serves as early-warning risk group

## Tools & Stack
Python, Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn

## Outcome
This segmentation framework enables data-driven financial decision making across marketing, risk, and customer service functions.

### KPI Visualizations

#### Average Customer Lifetime Value by Segment
<img width="564" height="455" alt="image" src="https://github.com/user-attachments/assets/d4dd50b3-6dc5-4286-a383-4e14a7670cba" />


#### Credit Risk Distribution by Segment
<img width="550" height="433" alt="image" src="https://github.com/user-attachments/assets/19aef184-d82d-4080-9bd8-54fbefa30ae1" />


