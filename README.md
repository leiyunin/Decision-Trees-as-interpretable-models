# Decision-Trees-as-interpretable-models

# Overview
This project delves into the realm of interpretable machine learning models, focusing on Decision Trees for classification and exploring LASSO and Boosting techniques for regression, across two different datasets:

- **Decision Trees on Acute Inflammations Dataset**:
  - **Data Acquisition**: Retrieves the Acute Inflammations dataset for analysis.
  - **Model Building**: Constructs a decision tree using the entire dataset and visualizes it to understand decision-making processes.
  - **Rule Conversion**: Translates decision tree branches into a series of IF-THEN rules for straightforward interpretability.
  - **Pruning**: Applies cost-complexity pruning to derive a minimal tree and a concise rule set, enhancing model interpretability without sacrificing accuracy.

- **LASSO and Boosting on Communities and Crime Dataset**:
  - **Dataset Preparation**: Utilizes the first 1495 rows as the training set, addressing missing values through data imputation and excluding non-predictive features.
  - **Feature Analysis**: Generates a correlation matrix and calculates the Coefficient of Variation (CV) for each feature, selecting those with the highest CV for further visualization and analysis.
  - **Regression Techniques**:
    - **Linear Model**: Employs least squares fitting on the training set, reporting test error.
    - **Ridge Regression**: Implements ridge regression, optimizing λ through cross-validation and evaluating test error.
    - **LASSO Regression**: Fits a LASSO model to identify key variables, performing the process with both raw and standardized features to compare test errors.
    - **Principal Component Regression (PCR)**: Adopts PCR, determining the optimal number of principal components via cross-validation.
    - **L1 Penalized Gradient Boosting Tree**: Uses XGBoost for building a gradient boosting tree with L1 penalized regression at each node, fine-tuning α (regularization term) through cross-validation.

This comprehensive analysis emphasizes the interpretability of decision trees and the efficacy of regularization and boosting in regression within high-dimensional spaces, showcasing the power of these techniques in extracting meaningful insights from complex datasets.