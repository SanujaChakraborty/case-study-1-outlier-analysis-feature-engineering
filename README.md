# case-study-1-outlier-analysis-feature-engineering
Data Science Case Study: Outlier analysis, missing value handling, feature engineering, feature importance, and model comparison (Regression + Classification).
# Case Study 1: Outlier Analysis, Missing Value Handling, Feature Engineering & Model Improvement

This repository contains the implementation and presentation for **Data Science Case Study 1** completed as part of my **M.Tech in AI & Data Science** program.

The objective of this case study was to analyze data quality issues, engineer useful features, identify important predictors, and compare the performance of multiple machine learning models for both regression and classification tasks.

---

## Contents of this Repository
/ppt/     → Presentation (Case Study 1 PPT)  
/code/    → Jupyter notebook / Python scripts  
/data/    → Sample dataset (optional)  
README.md → Project summary  


---

## 1. Handling Missing Values

Since the provided dataset contained no missing values, we **simulated missing values** to demonstrate different handling techniques.

### Technique Used: **Mean Imputation**
```
- Replaces missing values with the mean of the feature.
- Simple and effective when data is normally distributed.
- Helps maintain dataset size without dropping rows.
```
---

## 2. Outlier Detection using Boxplot

Outliers were detected using **Interquartile Range (IQR)** and visualized using boxplots.

### Key Concepts
```
- Q1 = 25th percentile  
- Q3 = 75th percentile  
- IQR = Q3 – Q1  
- Outliers = values outside:
```
**1.5 × IQR**

Boxplots helped visualize distribution & extreme values.

---

## 3. Feature Engineering

We applied transformations to improve model performance.

### Example: **Log Transformation**
Used to fix skewed distributions such as `log_crim`.
```
Effects:
- Reduces skewness  
- Makes the feature more normally distributed  
- Improves model stability
```
Visualized using histograms.

---

## 4. Feature Importance (Random Forest)

Random Forest was used to compute feature importance.

### Why Feature Importance Matters?
```
- Helps identify the most impactful features  
- Useful for dimensionality reduction  
- Improves interpretability  
- Allows model optimization by removing irrelevant variables  
```
We plotted a bar chart of feature importance and highlighted top 3 predictors.

---

## 5. Model Comparison (Regression)
```
We compared the following models:

- Linear Regression  
- Ridge Regression  
- Lasso Regression  
- Random Forest  
```
### Evaluation Metrics
```
- **MSE (Mean Squared Error)**  
- **R² Score**
```
### Findings
```
- **Random Forest performed best** with lowest MSE & highest R².
- Linear Regression underperformed due to its inability to model complex patterns.
- Ridge & Lasso provided moderate improvement through regularization.
```
---

## 6. Hyperparameter Tuning

Performed **Grid Search CV** to optimize hyperparameters.

### Example:
```
- Ridge Regression → Tuned **alpha**  
- Best alpha found: **1.0**
```

### Why Tuning Matters?
```
- Improves generalization  
- Reduces overfitting  
- Enhances model accuracy  
```
---

## Files Included
```
- PowerPoint presentation  
- Notebook/script for analysis  
- You may add datasets (optional)
```
---

## Author
**Sanuja Chakraborty**  
M.Tech (AI & DS)

---

## If you like this project, consider giving the repository a star!
