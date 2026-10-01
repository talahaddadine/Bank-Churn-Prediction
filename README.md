# Bank Customer Churn Prediction
A machine learning project completed at **German Jordanian University** in **2021**, predicting credit card customer attrition for a bank using classification models.

## Overview
Customer retention is critical in banking, where acquiring new customers is far more costly than retaining existing ones. This project builds a predictive pipeline to identify bank customers who are likely to cancel their credit card, so the bank can intervene with targeted retention efforts before losing them.

## Dataset

- **Source:** [Kaggle — BankChurners](https://www.kaggle.com/)
- **Size:** ~10,000 customers, 23 features
- **Target variable:** `Attrition_Flag` (Existing Customer vs. Attrited Customer)
- **Features include:** demographic data (age, gender, marital status, income), account data (card category, months on book, credit limit, utilization ratio), and transaction behavior (transaction amount/count and their change over time)

## Workflow

1. **Data cleaning** — dropped irrelevant/redundant columns, checked for missing values
2. **Exploratory data analysis** — visualized attrition patterns across demographics and account features using Pandas and Seaborn
3. **Encoding** — applied label encoding and one-hot encoding to convert categorical features to numerical values
4. **Train/test split** — 75% training / 25% testing using scikit-learn
5. **Modeling** — trained and tuned three classifiers:
   - K-Nearest Neighbors
   - Random Forest
   - XGBoost
6. **Evaluation** — compared models using accuracy, precision, recall, F1-score, and a confusion matrix

## Results

| Model | Accuracy |
|---|---|
| K-Nearest Neighbors | 88.6% |
| Random Forest | 96.3% |
| **XGBoost** | **96.4%** |

XGBoost was the best-performing model, correctly identifying the large majority of customers who churned (98% recall on the churn class).

## Tools & Libraries

- Python
- Pandas
- Seaborn
- scikit-learn
- XGBoost

## Authors

- Tala Haddadin
- Celine Alarmouti

School of Applied Technical Sciences, German Jordanian University
