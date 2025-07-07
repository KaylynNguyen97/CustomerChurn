# Customer Churn Prediction Using Machine Learning

## Overview
This repository contains an individual assignment focused on predicting customer churn for a banking institution using machine learning techniques. The goal is to build predictive models that can identify customers likely to leave the bank, enabling targeted retention efforts.

## Tools and Technologies
- **Programming Language**: Python
- **Environment**: Google Colab
- **Libraries**: 
  - scikit-learn
  - seaborn
  - matplotlib

## Dataset
- **Source**: Bank Churn Modeling (Kaggle)
- **Records**: 10,000 customer records
- **Features**: 
  - Age
  - Gender
  - HasCrCard
  - IsActiveMember
  - Exited (Target variable: 1 = churned, 0 = stayed)

## Business Questions
1. How can the bank predict customer churn before it happens?
2. How can we use ML models to help target retention efforts?
3. Which customers are most likely to leave the bank?

## Data Exploration and Analysis
- **Churn Rate**: Approximately 20%
- **Key Findings**:
  - Higher churn rates observed in Germany
  - Churn increases with age
  - Less active members are more likely to churn
  - Females have a higher churn rate

## Predictive Analytics
### Models Applied
- **Logistic Regression**
- **Support Vector Machine (SVM)**
- **Random Forest**

### Model Performance Overview
- **Random Forest**:
  - Accuracy: 87%
  - ROC AUC: 0.86
  - Recall: 48% (captures nearly half of churners)
  
- **Logistic Regression**:
  - Accuracy: 81%
  - Recall: 20%
  - Missed churners: 468 (high risk of revenue loss due to false negatives)
  
- **Support Vector Machine (SVM)**:
  - Accuracy: 86%
  - Recall: 38% (misses 62% of churners)
  - Lower false positives compared to Random Forest

### Key Takeaway
Prioritizing the detection of churners is crucial for customer retention strategies. The Random Forest model is the optimal choice due to its ability to identify more at-risk customers, despite having some false positives.

## Business Actions
1. Built machine learning models (especially Random Forest) to predict high-risk customers based on their behavior and attributes (age, geography, activity, etc.).
2. Used feature importance and exploratory data analysis (EDA) to identify high-risk groups (e.g., older customers, less active members, those from Germany).
3. Flagged high-risk customers for retention campaigns and reached out with personalized offers or loyalty incentives.

## Business Outcomes
- Focused marketing efforts based on model predictions.
- Reduced churn-related revenue loss and improved customer lifetime value.
- The Random Forest model correctly identified approximately 48% of churners, providing a tool to catch nearly half of potential leavers before they leave.

## Key Takeaways & Next Steps
- **Key Takeaways**:
  - Predictive modeling is effective for churn detection.
  - Random Forest is the best model for balancing accuracy and recall.
  
- **Next Steps**:
  - Deploy the model for real-time churn alerts.
