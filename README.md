# Regression
Machine Learning - Regressing Model Projects 

Regression models (both linear and non-linear) are used for predicting a real value, like salary for example. 
If the independent variable is time, then the model will be forecasting future values, otherwise the model will be predicting present but unknown values. 

There are multiple Machine Learning Regression models:
1. Simple Linear Regression
2. Multiple Linear Regression
3. Polynomial Regression
4. Support Vector for Regression (SVR)
5. Decision Tree Regression
6. Random Forest Regression

Evaluating fit of models with **R Squared**
![image](https://github.com/user-attachments/assets/0e780256-2d4c-4ef8-9c57-290ab05c53ac)
R² (R-squared) is a statistical measure that explains how well the independent variables in a regression model explain the variability of the dependent variable.

### Formula
The R² value is calculated as:

```
R² = 1 - (SSres / SStot)
```

Where:
- **SSres (Residual Sum of Squares):** Measures the error between the predicted and actual values.
- **SStot (Total Sum of Squares):** Measures the total variance in the data (difference from the mean).

### Interpreting R²
R² values range between **0 and 1**, where:

| R² Value | Interpretation |
|----------|---------------|
| **1.0**  | Perfect fit (model explains all variance) |
| **~0.9** | Very good fit |
| **0.7 - 0.9** | Acceptable fit |
| **0.4 - 0.7** | Poor fit (not great) |
| **< 0.4** | Very bad fit (terrible) |

### How Can R² Be Negative?
Although R² typically ranges between 0 and 1, it can be **negative** when the model fits the data worse than a simple horizontal line (mean of y-values). This happens when:
- The model does not capture the pattern in the data at all.
- The chosen independent variables have little to no relationship with the dependent variable.
- Overfitting or underfitting occurs.

### Effect of Adding More Independent Variables
- **Adding new independent variables can only decrease or maintain SSres** because we use **Ordinary Least Squares (OLS)**, which minimizes the sum of squared residuals.
- **SStot (Total Sum of Squares) does not change** because it depends only on y-values, not the independent variables.

### Adjusted R² (Improved R² Measure)
Adding more variables **always** increases R², even if the new variable is irrelevant. To address this, we use **Adjusted R²**:

```
Adjusted R² = 1 - ((1 - R²) * (n - 1) / (n - k - 1))
```

Where:
- **n** = Number of observations
- **k** = Number of independent variables

#### Advantages of Adjusted R²
- **Penalizes unnecessary variables** to prevent overfitting.
- **More reliable than R²** when comparing models with different numbers of predictors.
- **Used in model selection** to determine the best-performing regression model.

### Summary
- **Higher R² means a better model fit**, but context matters.
- **Adjusted R² is better for model evaluation**, especially when adding new variables.
- **R² can be negative** if the model performs worse than just using the mean.
