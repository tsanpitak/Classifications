# Unit 11—Risky Business



## Resampling

credit_risk_resampling.ipynb

Use Loan statistic from 2019 Q1 to create models to predict whether a loan will become a high-risk or low-risk loan. We'll be using logistic regression model, however, we'll be using four different methods to sample our data to train the model: Random Oversampling; SMOTE Oversampling; Cluster Centroids Undersampling; and Combination Sampling.

Which model had the best balanced accuracy score?
- Combination Sampling has the best balanced accuracy score
Which model had the best recall score?
- high risk - Cluster Centroids Undersampling 
- low risk - SMOTE Oversampling
- average - SMOTE Oversampling
Which model had the best geometric mean score?
- SMOTE Oversampling and Combination Sampling have the same score (highest) of 0.79.

## Ensemble Learning

In this section, you will train and compare two different ensemble classifiers to predict loan risk and evaluate each model. You will use the [Balanced Random Forest Classifier](https://imbalanced-learn.readthedocs.io/en/stable/generated/imblearn.ensemble.BalancedRandomForestClassifier.html#imblearn-ensemble-balancedrandomforestclassifier) and the [Easy Ensemble Classifier](https://imbalanced-learn.readthedocs.io/en/stable/generated/imblearn.ensemble.EasyEnsembleClassifier.html#imblearn-ensemble-easyensembleclassifier). Refer to the documentation for each of these to read about the models and see examples of the code.

Be sure to complete the following steps for each model:

1. Load the Lending Club data, split the data into training and testing sets, and scale the features data.
2. Train the model using the quarterly data from LendingClub provided in the `Resource` folder.
3. Calculate the balanced accuracy score from `sklearn.metrics`.
4. Print the confusion matrix from `sklearn.metrics`.
5. Generate a classification report using the `imbalanced_classification_report` from imbalanced learn.
6. For the balanced random forest classifier only, print the feature importance sorted in descending order (most important feature to least important) along with the feature score.

Use the above to answer the following:

> Which model had the best balanced accuracy score?
>
> Which model had the best recall score?
>
> Which model had the best geometric mean score?
>
> What are the top three features?

---

### Hints and Considerations

Use the quarterly data from the LendingClub data that is provided in the `Resources` folder. Keep the file in the zipped format and use the starter code to read the file.

Refer to the [imbalanced-learn](https://imbalanced-learn.readthedocs.io/en/stable/) and [scikit-learn](https://scikit-learn.org/stable/) official documentation for help with training the models. Remember that these models all use the model->fit->predict API.

For the ensemble learners, use 100 estimators for both models.

---

### Submission

* Create Jupyter notebooks for the homework and host the notebooks on GitHub.
* Include a markdown that summarizes your homework and include this report in your GitHub repository.
* Submit the link to your GitHub project to Bootcamp Spot.

---
