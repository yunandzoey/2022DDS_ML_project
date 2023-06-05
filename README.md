# Project: 2022DDS_ML_project
2022W RWTH DDS - Machine Learning Project -  Bankruptcy

# Problem: Bankruptcy Prediction

This data-set was obtained here: https://archive.ics.uci.edu/ml/datasets/Taiwanese+Bankruptcy+Prediction

It contains financial indicators about Taiwanese companies (from 1999 to 2009).
Each row contains 95 such indicators and one 0/1 label (binary classification).
The label tells whether or not the company went bankrupt.

## Data Status

* The data is **clean** (no missing values).
* The column names are well-descriptive of the features.
* The data is unbalanced: only around 3% of the companies went bankrupt.

## Recommendations

If you decide to re-balance classes using oversampling, remember to be careful about data leakage!
Python library "imblearn" has a lot of utilities to deal with imbalanced learning and it has a Pipeline class which is compatible with sklearn's Pipeline class.
Reference: https://imbalanced-learn.org/stable/auto_examples/pipeline/plot_pipeline_classification.html

After performing an initial data exploration, remember to only present in your project report the **interesting** findings, if any.
The presentation of data (via a textual description, tables or plots) should be short and informative.

In evaluating this project I am more interested in your correct application of model selection methodologies than in the performance of your model.

If your model has hyperparameters, I am more interested that your model selection procedure took them into account, even if you only try a few possible values for them.
Hyperparameter selection and model training shall not use all your computing resources for one week, but it should be set up "as if" you had access to a large computational infrastructure.
The only difference should be in the number of hyperparameter configurations evaluated; not in the rigour of the methodology used.

You should choose which classification metric to use (and motivate your choice!).
Reference: https://scikit-learn.org/stable/modules/model_evaluation.html#classification-metrics

# The algorithm used for this project:
1. Linear Regression: 
  - a statistical algorithm to model the relationship between dependent variables and one or multiple independent variables.
  - to find a best-fitting line that minimises the sum of square residuals between the line and data.
  - commonly used for predicting continuous numerical values
2. Logistic Regression: 
  - a classification algorithm to model the relationship between independent variables and the probability of a binary outcome by logistic function(sigmoid function).
  - to etimate the parameters that maximize the likelihood of the observed data.
  - to outcome the probability of positive class ( also for multi-class problem)
3. Decision Tree Classification
  - a non-parametric supervised machine-learning algorithm to crease a tree-like model to make predictions.
  - partitions the feature space based on the values of different input features, 
  - constructure a tree structure where each node represents a decision based on a feature, and each leaf node represents a class label or a prediction, 
  - is intuitive and can handle both numerical and categorical data.
4. K Neighborhoods Classifier
5. Random Forest 
7. XGB Classifier
