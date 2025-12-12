# Customer Churn Prediction & Retention Strategy Using Machine Learning and Clustering
This project uses machine learning (XGBoost, Random Forest) and customer segmentation tools to predict churn and improve customer retention for a business.

---
## Executive Summary

This project focuses on solving a common problem in the industry — customer churn. I built a churn prediction model, analyzed key features, grouped users by behavior, and gave clear strategies to improve retention.

- **Problem**: A company faces high customer churn rates, hurting long-term growth.
- **Solution**: I used machine learning to predict churn and clustering to group users by risk.
- **Results**: 
  - Model accuracy reached **80%** after threshold tuning
  - XGBoost correctly identified **59% of churned customers**, allowing the business to take early action
  - The model also predicted **86% of stayed customers** correctly, helping focus on upselling and referral strategies
  - Customer segmentation revealed a **high‑risk group with a 32% churn rate**
  - Provided clear and personalized retention plans for each customer segment
- **Next steps**: Add more real-time data, A/B test retention campaigns
- **Business Value**: Better user understanding, targeted strategies, and improved customer lifetime value (LTV)

---
## Business Problem

### Why this project?
A company often loses customers because they don’t understand who is at risk and why. This costs money and slows growth.

### Why does it matter?
Improving retention increases profits and is cheaper than getting new customers. Understanding churn helps build better services.

### What am I solving?
Predict who is likely to leave and find patterns in their behavior. This helps the business take action early.

---
## Methodology

- **Churn Prediction**: Used XGBoost and Random Forest to predict if a customer will leave.
- **Feature Analysis**: Found which factors affect churn the most (e.g., balance, age, gender).
- **Customer Segmentation**: Used K-Means clustering to group customers by risk.

---
## Specific Skills Used

- **Python**: pandas, numpy, scikit-learn, xgboost, matplotlib, seaborn
- **Machine Learning**: XGBoost, Random Forest, classification report, confusion matrix, ROC/PR curve
- **Clustering**: K-Means, Elbow method, Silhouette Score, PCA visualization
- **Data Analysis**: Feature engineering, correlation analysis, risk labeling
- **Business Thinking**: Designed retention strategies based on user risk level

---
## Results & Business Recommendation

### What I found:
- **Key churn signals**: 
  - **Age**: Both models ranked customer **age** as the most important factor. Older users tend to have higher churn probability.
  - **Balance**: High account balance was a key signal, especially in **Group 2**, which has the highest average balance and churn rate (32.4%).
  - **Gender and Geography**: XGBoost showed **being male** and **from Germany** increased churn risk.
  - **Tenure**: Customers with **shorter time with the company** also showed higher churn tendencies.
  
- **Three customer groups**:
  - Group 0: Low risk (16% churn), loyal core users
  - Group 1: Low risk (17%), potential to grow
  - Group 2: High risk (32%), urgent to retain

### What I suggest:
- Group 0: Offer upgrade plans, encourage referrals
- Group 1: Improve user onboarding and collect feedback
- Group 2: Give special discounts, optimize user experience

These actions can increase customer lifetime value and reduce churn loss.

---
## Next Steps

### If I had more time:
- Add more features: usage frequency, support tickets, marketing data
- Try more models: Logistic Regression, LightGBM, Neural Networks
- Test strategies: Run A/B tests on retention campaigns

### Limitations:
- The dataset is simulated and may not reflect all real-world behaviors
- Limited time-based data (no trends over time)
- No external variables (e.g. competitor impact, pricing changes)

---
## Data Source

This project uses the **Customer Churn** dataset from [Kaggle](https://www.kaggle.com/datasets/willianoliveiragibin/customer-churn/data).

The dataset includes **10,000 customer records**, with details such as:
- Age, Gender, Geography
- Credit Score, Tenure
- Balance, Estimated Salary
- Whether the customer has churned or not

It is commonly used for churn prediction projects and machine learning practice.
