# Data Quality Report

## 1. Missing Values

Several datasets contained missing values in behavioral and engagement-related columns. Missingness patterns were reviewed to assess their potential impact on downstream analysis.

## 2. Duplicate Records

Duplicate checks were performed across major datasets. No significant duplicate customer or order records were identified.

## 3. Invalid or Unusual Values

Data distributions were inspected for unrealistic order amounts, abnormal activity counts, and inconsistent categorical values.

## 4. Outlier Analysis

Outliers were identified in monetary and behavioral variables such as order amount and session activity. These observations may represent high-value customers or abnormal user behavior.

## 5. Join Integrity Checks

Customer identifiers were validated across datasets. All order records successfully mapped to valid customer IDs, indicating strong referential consistency.

## 6. Date Consistency Checks

Date ranges across signup activity and order history were reviewed. No major future-dated or historically inconsistent records were identified.

## 7. Potential Data Leakage Risks

Certain behavioral variables may contain future information or post-event patterns that could unintentionally leak churn outcomes during predictive modeling. Care should be taken during feature selection.