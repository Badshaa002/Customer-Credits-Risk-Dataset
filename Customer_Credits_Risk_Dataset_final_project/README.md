# 📊 Customer Credits Risk Dataset

Professional data preprocessing and feature engineering project built for a customer credit risk prediction use case.

## ✨ Project Overview

This repository contains a complete end-to-end preprocessing workflow for a **Customer Credit Risk Dataset**.  
The project shows how raw data from multiple sources can be cleaned, merged, transformed, and prepared for machine learning.

The work includes:

- Loading data from **CSV, JSON, SQL, and a dummy API source**
- Handling missing values using multiple techniques
- Detecting and treating outliers
- Encoding categorical variables
- Scaling numerical features
- Creating new useful features
- Preparing a final dataset ready for ML modeling

## 🎯 Objective

The goal of this project is to prepare a clean and structured dataset that can be used to predict whether a customer is likely to **default on a loan**.

## 🧩 Problem Statement

In this project, the dataset contains customer demographic, financial, and behavioral information.  
The target column is **`default_flag`**, where:

- `0` = No Default
- `1` = Default

The complete preprocessing pipeline was built to improve the dataset quality before machine learning.

## 🔄 Workflow Covered

### 1. Data Acquisition

- CSV file for transaction and loan details
- JSON file for customer metadata
- SQL database for repayment history
- Dummy API file for regional economic indicators

### 2. Data Understanding and Cleaning

- `info()` and `describe()`
- Data profiling report
- Missing value analysis
- Simple imputation
- Most frequent imputation
- Random sample imputation
- KNN imputation
- MICE imputation
- Complete case analysis

### 3. Outlier Handling

- Z-score method
- IQR method
- Percentile capping
- Winsorization

### 4. Feature Engineering

- Date feature extraction
- Ordinal encoding
- Label encoding
- One-hot encoding
- Binning
- Binarization
- K-Means binning

### 5. Feature Scaling and Transformation

- StandardScaler
- Normalizer
- MinMaxScaler
- MaxAbsScaler
- RobustScaler
- Log transform
- Reciprocal transform
- Square-root transform
- Box-Cox transform
- Yeo-Johnson transform

### 6. Final Deliverable

- Final cleaned dataset
- Summary report
- Data quality report
- Notebook with outputs and interpretations

## 📁 Repository Structure

```text
holistic_data_preparer_final_project/
├── Customer Credits Risk Dataset.ipynb
├── README.md
├── SUMMARY_REPORT.md
├── data/
│   ├── api_economic_indicators.json
│   ├── customer_metadata.json
│   ├── customer_transactions.csv
│   └── loan_repayment.db
├── outputs/
│   ├── data_quality_report.html
│   └── final_cleaned_transformed_dataset.csv
└── screenshots/
    ├── 1 B-source summery.png
    ├── 2 C-data u&c.png
    ├── 3 D- outliers.png
    ├── 4 E- feature engg.png
    ├── 5 F-feature scalling.png
    ├── 6 G- features const & trans 1.png
    ├── 6 G- features const & trans 2.png
    └── 7 H-final dataset.png
```

## 🛠️ Tools and Libraries

- Python
- Pandas
- NumPy
- Scikit-learn
- SQLite
- Jupyter Notebook
- ydata-profiling

## 📌 Main Files

- 📘 Notebook: [Customer Credits Risk Dataset.ipynb](./Customer%20Credits%20Risk%20Dataset.ipynb)
- 📝 Summary Report: [SUMMARY_REPORT.md](./SUMMARY_REPORT.md)
- 📂 Source Data: [data](./data)
- 📤 Final Output: [final_cleaned_transformed_dataset.csv](./outputs/final_cleaned_transformed_dataset.csv)
- 📈 Data Quality Report: [data_quality_report.html](./outputs/data_quality_report.html)

## 📊 Final Results

| Metric | Value |
|---|---|
| Final dataset size | **60 rows × 43 columns** |
| Missing values after preprocessing | **0** |
| Data sources used | **4** |
| Notebook cells | **72** |
| Final dataset status | **Ready for ML** |

## 🖼️ Project Screenshots

### 📥 Data Source Summary

![Data Source Summary](./screenshots/1%20B-source%20summery.png)

This screenshot shows the summary of the source files used in the project.

### 🧹 Data Understanding and Cleaning

![Data Understanding and Cleaning](./screenshots/2%20C-data%20u%26c.png)

This section shows dataset inspection and missing value handling steps.

### 📉 Outlier Handling

![Outlier Handling](./screenshots/3%20D-%20outliers.png)

This screenshot highlights the outlier detection and treatment stage.

### 🏗️ Feature Engineering

![Feature Engineering](./screenshots/4%20E-%20feature%20engg.png)

This stage includes encoding, binning, and creation of new useful features.

### ⚖️ Feature Scaling

![Feature Scaling](./screenshots/5%20F-feature%20scalling.png)

This screenshot shows the scaling methods applied to numerical features.

### 🔁 Feature Construction and Transformation

![Feature Construction and Transformation - 1](./screenshots/6%20G-%20features%20const%20%26%20trans%201.png)

![Feature Construction and Transformation - 2](./screenshots/6%20G-%20features%20const%20%26%20trans%202.png)

These screenshots show feature construction and transformation steps used before the final dataset export.

### ✅ Final Dataset

![Final Dataset](./screenshots/7%20H-final%20dataset.png)

This screenshot shows the final processed dataset ready for machine learning.

## 🚀 How to Run

1. Open the notebook [Customer Credits Risk Dataset.ipynb](./Customer%20Credits%20Risk%20Dataset.ipynb)
2. Select the correct Python/Jupyter kernel in VS Code or Jupyter
3. Run the notebook cells from top to bottom
4. Check the `outputs/` folder for the generated files

## 📦 Deliverables

- Complete Jupyter Notebook
- Final cleaned and transformed dataset
- Data quality profiling report
- Summary report
- Screenshot evidence for submission

## 🏁 Conclusion

This project demonstrates a full preprocessing workflow for credit risk data in a clear and structured way.  
The final dataset is cleaned, transformed, and ready to be used in a machine learning model for loan default prediction.
