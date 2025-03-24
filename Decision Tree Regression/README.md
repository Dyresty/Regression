## Classification and Regression Trees - CART
Consists of Classification Trees and Regression Trees. 

# Regression Tree vs Classification Tree

Decision Trees are powerful supervised learning models used for both **Regression** and **Classification** tasks.

## 1. Regression Tree
- **Purpose:** Predicts **continuous** numerical values.
- **Target Variable:** Continuous (e.g., house price, temperature, salary).
- **Splitting Criterion:** Reduces variance (e.g., using **Mean Squared Error (MSE)** or **Mean Absolute Error (MAE)**).
- **Prediction Output:** A numerical value (average of the target values in the leaf node).

### Example:
Predicting house prices based on area, number of rooms, and location.

## 2. Classification Tree
- **Purpose:** Predicts **categorical** labels (classes).
- **Target Variable:** Categorical (e.g., spam/not spam, fraud/no fraud).
- **Splitting Criterion:** Maximizes information gain (e.g., using **Gini Index** or **Entropy**).
- **Prediction Output:** A class label (majority class in the leaf node).

### Example:
Classifying emails as **spam** or **not spam** based on keywords and sender information.

## Key Differences

| Feature            | Regression Tree  | Classification Tree  |
|-------------------|----------------|------------------|
| **Output Type**   | Continuous values | Discrete class labels |
| **Target Variable** | Numerical | Categorical |
| **Splitting Criterion** | Reduces variance (MSE, MAE) | Increases purity (Gini, Entropy) |
| **Leaf Node Prediction** | Mean/average of values | Majority class label |
| **Example Use Case** | Predicting house prices | Classifying emails as spam or not |

# Regression Decision Tree 
- These can be used for datasets with hundreds of features, it will work well for them.
- If the dataset needs encoding of categorical data or missing data, perform preprocessing work.<br>
In encoding<br>
**Label Encoder** - If order matters.<br>
**Column Transformer** - If order does not matter.<br>
- Feature scaling is not required for both Decision Tree Regression and Random Forest Regression.<br>
Predictions from these models are resulting from the successive splits of the data through the different of the tree, and do not involve equations like the other regression models.
