# Credit Card Fraud Detection

## Overview

This project aims to detect credit card fraud using machine learning techniques. The dataset used for this project is available [here](https://colab.research.google.com/drive/1Y2zfI-6J3rBhDhq8_s3rzF8W_-SKCdcG).

## Libraries Used

- `pandas` - Data manipulation and analysis.
- `numpy` - Numerical computations.
- `matplotlib` - Data visualization.
- `seaborn` - Statistical data visualization.
- `sklearn.ensemble` - Includes `RandomForestClassifier` and `ExtraTreesClassifier` for classification models.
- `sklearn.tree` - Includes `DecisionTreeClassifier`.
- `sklearn.metrics` - Metrics for model evaluation, including `confusion_matrix` and `accuracy_score`.
- `sklearn.model_selection` - Includes `KFold`, `StratifiedKFold`, and `RandomizedSearchCV` for model selection and hyperparameter tuning.
- `sklearn.preprocessing` - Includes `StandardScaler` for feature scaling.

## Execution Methodology

1. **Import Libraries**: Import necessary Python libraries for data manipulation, model building, and evaluation.

2. **Import Dataset**: Load the credit card fraud dataset from the specified CSV file.

3. **Data Analysis**:
   - Display basic information about the dataset, such as shape, info, and any missing values.
   - Analyze the distribution of the target variable `Class`.

4. **Feature Selection and Importance**:
   - Use `ExtraTreesClassifier` to determine feature importances.
   - Select the top 18 most important features based on the feature importance scores.

5. **Data Splitting**:
   - Split the dataset into training and test sets using `StratifiedKFold` cross-validation.

6. **Model Selection**:
   - Define `DecisionTreeClassifier` and `RandomForestClassifier` models for classification.

7. **Hyperparameter Tuning for RandomForestClassifier**:
   - Define a grid of hyperparameters for `RandomForestClassifier`.
   - Perform randomized search for hyperparameter tuning (code commented out).

8. **AutoML using LazyPredict**:
   - (Optional) Use `LazyPredict` to quickly evaluate various classifiers (code commented out).

9. **Model Evaluation**:
   - Fit the `RandomForestClassifier` model to the training data.
   - Predict on the test data and evaluate the model's accuracy.





