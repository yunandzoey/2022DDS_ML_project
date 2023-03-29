# 2022DDS_ML_project
2022W RWTH DDS - Machine Learning Project -  Bankruptcy

# Bankruptcy Prediction

This data-set was obtained here: https://archive.ics.uci.edu/ml/datasets/Taiwanese+Bankruptcy+Prediction

It contains financial indicators about Taiwanese companies (from 1999 to 2009).
Each row contains 95 such indicators and one 0/1 label (binary classification).
The label tells whether or not the company went bankrupt.

## Highlights

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
