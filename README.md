# Breast Cancer Classification

Personal learning project, separate from the selection cases. It compares simple classification baselines on scikit-learn's copy of the Wisconsin Diagnostic Breast Cancer dataset. The notebook treats malignant as the positive class and reports complementary classification metrics.

## Method

- Hold out 20% of observations with stratification and a fixed random seed.
- Keep scaling inside the Logistic Regression pipeline so it learns from training data only.
- Compare malignant-class precision, recall, and F1 with balanced accuracy, ROC AUC, average precision, and confusion matrices.
- Use one fixed holdout split. The notebook does not tune hyperparameters, estimate confidence intervals, or calibrate predicted probabilities.

## Dataset

The notebook loads the dataset with `sklearn.datasets.load_breast_cancer`; it does not redistribute a separate CSV. Scikit-learn documents 569 observations, 30 numeric features, and its source as the [UCI Wisconsin Diagnostic Breast Cancer dataset](https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic). See the [scikit-learn loader documentation](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_breast_cancer.html) for the returned target labels and dataset details.

## Run

Use Python with pandas, scikit-learn, and Jupyter installed. Open `breast_cancer_prediction.ipynb` and run the cells in order. The dataset comes from the scikit-learn package.

## Limitations

This small educational dataset does not represent a clinical workflow or current patient population. The single holdout scores do not establish generalization, clinical utility, or safety. The project is for learning only and must not guide diagnosis or care.
