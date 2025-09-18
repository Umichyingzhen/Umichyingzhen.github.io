---
title: "MLST: Statistical Analysis and Regression Tools in R"
excerpt: "Developed an R package to compute regression statistics and test results including Residual Standard Error, R-squared, Adjusted R-squared, F-test, and T-test."
collection: portfolio
date: 2024-11-15
---

---

### 📦 Project Summary

- **Objective**: Provide statistical tools for linear regression analysis in R through a user-friendly package.  
- **Key Functions**: Residual Standard Error, `R^2`, Adjusted `R^2`, F-test, T-test.  
- **Implementation**: Built in R with functions that directly take response and predictor matrices with a data frame.  
- **Main Finding**: Functions reproduce regression statistics consistent with `lm()` output, providing lightweight alternatives with simplified inputs.

---

### 📈 Usage Example

<img src="/files/MLST_Usage.png" alt="Usage example of MLST functions in R" style="width:100%;"/>

> - Demonstrates running all five functions on a simulated dataset with predictors \(X_1, X_2\) and response `normal`.  
> - Outputs include RSE, \(R^2\), adjusted \(R^2\), F-test table (F-statistic, p-value, df1, df2), and T-test matrix (estimate, SE, t, p).  
> - Results are consistent with base R regression output, validating correctness of the package implementation.  

---

### 📋 Table Results

| Function | Output Type | Key Values Returned |
|----------|-------------|---------------------|
| RSE      | Numeric     | Residual Standard Error |
| Rsquared | Numeric     | \(R^2\) value |
| ADJRS    | Numeric     | Adjusted \(R^2\) |
| Ftest    | Data frame  | F-statistic, p-value, df1, df2 |
| Ttest    | Matrix      | Estimate, SE, t-value, p-value |

> - Each function provides focused outputs instead of the full regression summary.  
> - The separation of tasks allows flexible and modular use of regression statistics in analysis workflows.  

---

### 📎 Full Package

👉 [[MLST Package]](https://github.com/Umichyingzhen/MLST)
