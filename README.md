## Summary of Steps

1. **Data Preparation**:
   - Load data from Excel files and merge them.
   - Handle missing values by dropping rows with specific values.

2. **Feature Selection**:
   - Use chi-square test for categorical features and ANOVA for numerical features.
   - Retain features with significant associations with the target variable.

3. **Data Encoding**:
   - Label encode categorical features and perform ordinal encoding for 'EDUCATION'.
   - Apply one-hot encoding to convert categorical features into binary format.

4. **Machine Learning Model Fitting**:
   - Train Random Forest, Decision Tree, and XGBoost classifiers.
   - Evaluate model performance using accuracy, precision, recall, and F1-score.

5. **Model Improvement**:
   - Explore hyperparameter tuning for the XGBoost classifier using techniques like grid search.
   - Perform a wide search over combinations of hyperparameters, e.g., around 900 combinations, to find optimal settings for the XGBoost model.

6. **XGBoost Model Improvement**:

This XGBoost setup stands out:

- **colsample_bytree:** 0.9
- **learning_rate:** 1
- **max_depth:** 3
- **alpha:** 1
- **n_estimators:** 50

Achieving 81% accuracy on the training set and 78% on the testing set.

