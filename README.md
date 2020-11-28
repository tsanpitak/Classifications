# Unit 11—Risky Business

## Resampling

credit_risk_resampling.ipynb

Use Loan statistic from 2019 Q1 to create models to predict whether a loan will become a high-risk or low-risk loan. We'll use logistic regression model, however, we'll be using four different methods to sample our data to train the model: Random Oversampling; SMOTE Oversampling; Cluster Centroids Undersampling; and Combination Sampling.

Which model had the best balanced accuracy score?
- Combination Sampling has the best balanced accuracy score
Which model had the best recall score?
- high risk - Cluster Centroids Undersampling 
- low risk - SMOTE Oversampling
- average - SMOTE Oversampling
Which model had the best geometric mean score?
- SMOTE Oversampling and Combination Sampling have the same score (highest) of 0.79.

## Ensemble Learning

credit_risk_ensemble.ipynb

Use Loan statistic from 2019 Q1 to create models to predict whether a loan will become a high-risk or low-risk loan. We'll use 2 ensemble models: Balance Random Forest model and Easy Ensemble model.

Which model had the best balanced accuracy score?
- Easy Emsemble
Which model had the best recall score?
- high risk - Easy Ensemble
- low risk - Easy Ensemble
- average - Easy Ensemble
Which model had the best geometric mean score?
- Easy Ensemble
What are the top three features?
- total_rec_prncp: (0.08322179913812433)
- total_pymnt_inv: (0.06904406031487648)
- last_pymnt_amnt: (0.061119989899441445)
---
