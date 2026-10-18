# Breast Cancer Classification

An educational classification project using the Wisconsin Diagnostic Breast Cancer dataset. It compares Logistic Regression and Random Forest on a stratified holdout set.

## Method

- Keep the patient identifier out of the feature set.
- Split the original observations before any resampling.
- Fit preprocessing on the training split only.
- Report precision, recall, F1, ROC AUC, and the confusion matrix. Treat results as a learning exercise, not as clinical evidence.

## Data and source

The repository includes the dataset distributed with the original project. The source is the [Wisconsin Diagnostic Breast Cancer dataset on Kaggle](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data). Check its current license and attribution requirements before republishing the dataset.

## Run

Open `breast_cancer_prediction.ipynb` from this directory. The notebook expects `data.csv` beside it. Install the notebook's Python imports in your own environment before running it.
