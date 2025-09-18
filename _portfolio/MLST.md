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

### 📎 Installation

👉 [[MLST Package GitHub]](https://github.com/Umichyingzhen/MLST)

👉 
    ```r
# 1) Install remotes (if not already installed)
install.packages("remotes")

# 2) Install the MLST package
remotes::install_github("Umichyingzhen/MLST")

# 3) Load and quickly verify
library(MLST)

