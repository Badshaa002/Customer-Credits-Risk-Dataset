# Final Project Summary Report

## Project Title
Holistic Data Preparer - Customer Credit Risk Dataset

## Objective
The aim of this project was to collect customer credit data from multiple sources, clean the data, handle missing values and outliers, apply feature engineering, and prepare a final dataset for machine learning.

## Data Sources Used
- CSV file for transaction and loan details
- JSON file for customer metadata
- SQL database for repayment history
- Dummy API JSON for external regional indicators

## Data Cleaning Summary
- Missing values were found in `age`, `gender`, `employment_type`, `annual_income`, `loan_amount`, and `credit_score`.
- Different methods were demonstrated: median imputation, most frequent imputation, random sample imputation, KNN imputation, MICE, and complete case analysis.
- For the final dataset, categorical values were filled with mode and important numeric columns were filled using KNN imputation.

## Outlier Handling Summary
- Outliers were checked using Z-score, IQR, percentile capping, and winsorization.
- Winsorization with the 5th and 95th percentile limits was used in the final cleaned version.

## Feature Engineering Summary
- Date features created: join year, join month, join day, join weekday
- Encodings used:
  - Ordinal encoding for education level
  - Label encoding for gender
  - One-hot encoding for region, loan purpose, and employment type
- New features created:
  - Debt-to-income ratio
  - Average monthly transactions
  - Spending-to-income ratio
  - Log, square-root, and reciprocal spending transforms
  - Box-Cox and Yeo-Johnson power transforms

## Scaling Summary
The notebook demonstrates StandardScaler, Normalizer, MinMaxScaler, MaxAbsScaler, and RobustScaler. The final dataset uses RobustScaler because it is more stable when outliers are present.

## Final Output
- Original missing values in main CSV source: 12
- Missing values after final preprocessing: 0
- Final dataset shape: 60 rows x 43 columns
- Final dataset file: `outputs/final_cleaned_transformed_dataset.csv`

## Conclusion
The dataset was successfully cleaned and transformed. It is now complete, consistent, and suitable for use in a machine learning model for loan default prediction.
