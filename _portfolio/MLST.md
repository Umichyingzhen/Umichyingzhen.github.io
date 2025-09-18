---
title: "MLST: Statistical Analysis and Regression Tools in R"
excerpt: "R package for obtaining statistical results from linear regression models, including residual standard error, R-squared, adjusted R-squared, F-tests, and T-tests."
collection: portfolio
date: 2025-09-17
---

This is an R package project developed by Yingzhen Wang.  
GitHub repository: [Umichyingzhen/MLST](https://github.com/Umichyingzhen/MLST)

---

### 📦 Package Features

- **Residual Standard Error (RSE)**: Compute the residual standard error for linear regression models.  
- **R-Squared (\(R^2\))**: Calculate the coefficient of determination to assess model fit.  
- **Adjusted R-Squared**: Evaluate the adjusted \(R^2\), accounting for the number of predictors in the model.  
- **F-test**: Evaluate the overall significance of a multiple linear model, including F-statistic, p-value, and degrees of freedom.  
- **T-test**: Evaluate the significance of individual predictors, including estimate, standard error, t-statistic, and p-value.  

---

### ⚙️ Installation

```r
# Install remotes if not already installed
install.packages("remotes")

# Authorization of package from GitHub (replace "auth_token" with your token)
Sys.getenv("GITHUB_PAT")
Sys.setenv(GITHUB_PAT = "auth_token")
nchar(remotes:::github_pat())

# Install MLST from GitHub
remotes::install_github("Umichyingzhen/MLST")
