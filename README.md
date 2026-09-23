# 🏦 Bank Customer Churn Analysis

## 📑 Table of Contents

- [Overview](#-overview)
- [Objectives](#-objectives)
- [Tools & Technologies](#-tools--technologies)
- [Project Workflow](#-project-workflow)
- [Machine Learning Models](#-machine-learning-models)
- [Model Performance](#-model-performance)
- [Key Insights](#-key-insights)
- [Business Recommendations](#-business-recommendations)
- [Conclusion](#-conclusion)
- [Project Files](#-project-files)

---

## 📋 Overview

Customer churn is a critical problem for banks because losing existing customers can impact revenue and long-term customer relationships.

This project analyzes bank customer data to uncover patterns associated with churn and builds machine learning models to identify customers at higher predicted risk of churn, enabling proactive and targeted retention efforts.

---

## 🎯 Objectives

- Analyze customer characteristics and churn patterns
- Perform data cleaning and exploratory data analysis (EDA)
- Identify the factors most strongly associated with churn predictions
- Build classification models to predict customer churn
- Compare model performance using accuracy, precision, recall, and F1-score
- Translate analytical findings into concrete business recommendations

---

## 🛠 Tools & Technologies

| Category | Tools |
|---|---|
| Language | Python |
| Data Handling | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn |
| Environment | Jupyter Notebook |

---

## 🔄 Project Workflow

1. Data Cleaning
2. Exploratory Data Analysis
3. Feature Engineering
4. Categorical Variable Encoding
5. Train-Test Split
6. Feature Scaling
7. Logistic Regression
8. Random Forest
9. Balanced Random Forest
10. Model Evaluation
11. Feature Importance
12. Business Insights
13. Business Recommendations

---

## 🤖 Machine Learning Models

### Logistic Regression

Used as a baseline classification model.

### Random Forest

Used to capture nonlinear relationships between customer characteristics and churn.

### Balanced Random Forest

A class-weighted Random Forest used to address the imbalance between churned and non-churned customers.

---

## 📊 Model Performance

| Model | Accuracy | Churn Precision | Churn Recall | Churn F1 |
|---|---:|---:|---:|---:|
| Logistic Regression | 81.00% | 59.71% | 20.39% | 30.40% |
| Random Forest | 86.55% | 77.60% | 47.67% | 59.06% |
| Balanced Random Forest | 84.75% | 63.00% | 60.00% | 62.00% |

The Balanced Random Forest trades some overall accuracy for a substantial improvement in churn recall, reaching approximately 60%. This means it identifies a larger proportion of actual churned customers compared with the other models tested.

For a retention-focused use case, the Balanced Random Forest provides a useful trade-off between identifying churned customers and maintaining prediction precision.

---

## 🔍 Key Insights

- Age was the most important feature according to the Random Forest feature-importance analysis.
- Estimated salary, credit score, balance, and number of products were also important features for the model.
- Customer activity level was relevant to churn prediction.
- Churn rates varied across countries in the analyzed dataset.
- The dataset showed a class imbalance between churned and non-churned customers.

---

## 💡 Business Recommendations

- **Target high-risk customer segments:** Use predicted churn risk to identify customers who may require targeted retention strategies.
- **Increase customer engagement:** Encourage less-active customers to use relevant banking services through personalized offers and reminders.
- **Improve product engagement:** Monitor customers with limited product usage and provide relevant product recommendations.
- **Analyze regional churn:** Investigate differences in churn across countries and develop location-specific retention strategies.
- **Use churn prediction proactively:** Use the Balanced Random Forest as an early-warning system to prioritize customers for retention efforts.

---

## ✅ Conclusion

This project demonstrates how exploratory data analysis and machine learning can be used to analyze and predict customer churn.

Three classification models were evaluated: Logistic Regression, Random Forest, and Balanced Random Forest. The Balanced Random Forest improved churn detection, achieving a churn recall of approximately 60% and an F1-score of 62%.

The analysis identified important features for the model's churn predictions, including age, estimated salary, credit score, balance, and number of products.

These findings can help banks identify customers at higher predicted risk of churn and prioritize targeted retention strategies.

---

## 📁 Project Files

- `bank_churn_customers.ipynb` — Complete data analysis, visualizations, machine learning models, model evaluation, business insights, and recommendations.
