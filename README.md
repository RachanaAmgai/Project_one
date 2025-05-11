# Project_one

**Authors**: Rachana Amgai, Baldwin Dyce, Isis Lara  
**Date**: may 11 , 2025

---
#  Multi-level Classification ML Project: Predicting Customer Churn

This repository presents a comprehensive machine learning project focused on predicting customer churn in the telecommunications industry using multi-level classification techniques. The goal is to not only identify which customers are likely to churn but also to predict the specific **category** and **reason** for churn, enabling targeted retention strategies.

---

##  Project Overview

Customer churn—the rate at which customers stop using a company's services—is a critical metric for telecommunication businesses. High churn can significantly impact revenue and growth.

By leveraging machine learning, this project aims to:

-  Predict if a customer will churn  
-  Classify the churn category (e.g., service, price, support)  
-  Identify the specific churn reason (e.g., network issues, billing disputes)

This **multi-level approach** enables proactive intervention and improved customer retention.

---

##  Business Impact

- **Increase Revenue**: Retaining customers reduces lost revenue and the need for costly acquisition campaigns.
- **Optimize Acquisition Costs**: Preventing churn lowers the cost per customer by reducing the need to win back lost users.
- **Enhance Customer Satisfaction**: Understanding churn drivers allows for targeted improvements in service and customer experience.

---

##  Project Approach

### 1. Data Exploration & Preprocessing
- **EDA**: Understand data distribution, missing values, and feature relevance.
- **Missing Data Handling**: Drop or impute values as appropriate.
- **Feature Engineering**: 
  - Remove irrelevant IDs and columns
  - Encode categorical variables using label encoding (to avoid dimensionality explosion)
  - Balance dataset with SMOTE or undersampling

### 2. Problem Formulation
- **Multi-class Classification**: Predict the churn category (e.g., "Not Applicable" for non-churners).
- **Multi-label Classification**: Predict both the churn category and churn reason (as customers may have multiple reasons).

### 3. Model Selection
- **Baseline Models**: Decision Trees, Logistic Regression
- **Ensemble Methods**: Random Forest, Bagging, Boosting (e.g., XGBoost)
- **Deep Learning**: MLP (Multi-layer Perceptron) using Keras/TensorFlow for complex patterns

### 4. Model Training & Evaluation
- **Supervised Learning**: Trained on labeled historical customer data
- **Evaluation Metrics**: 
  - F1-score, Recall, Precision  
  - Confusion Matrix, ROC AUC  
  - Emphasis on **F1-score and Recall** due to class imbalance

- **Avoid Data Leakage**: All preprocessing is split between training and test datasets.

---

##  Key Concepts

| Task Type               | Description                                                        | Example Algorithms         |
|------------------------|--------------------------------------------------------------------|----------------------------|
| Multi-class Classification | Assigns one label from multiple possible categories to each instance | Logistic Regression, RF    |
| Multi-label Classification | Assigns multiple labels (e.g., churn category & reason) to each instance | Neural Networks, Ensemble |

---

##  Workflow Summary

1.  **Data Exploration**: Visualize and analyze the dataset
2.  **Preprocessing**: Clean data, encode features, balance classes
3.  **Modeling**: Train & tune models for classification tasks
4.  **Evaluation**: Assess models using business-prioritized metrics
5.  **Deployment** *(optional)*: Package best model for integration

---

##  Tools & Libraries

- **Python**: Primary language
- **Pandas, NumPy**: Data manipulation
- **Scikit-learn**: ML models and evaluation
- **Imbalanced-learn**: SMOTE and undersampling
- **Keras / TensorFlow**: Deep learning
- **Matplotlib / Seaborn**: Visualization
  
## Conclusion
This project provides a robust ML framework for telecom companies to predict customer churn at multiple levels, offering actionable insights into churn likelihood, category, and reasons. By adopting this strategy, businesses can reduce churn, enhance customer satisfaction, and drive sustainable growth.


##  Ethical Considerations

- Balanced the dataset to prevent majority class bias.
- Monitored feature importances to avoid unfair targeting based on protected attributes.
- Focused on interpretable models to enable transparent business decisions.

---

