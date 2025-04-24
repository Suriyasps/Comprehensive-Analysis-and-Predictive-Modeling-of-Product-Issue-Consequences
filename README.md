# Comprehensive Analysis and Predictive Modeling of Product Issue Consequences

## 📌 Objective

This project focuses on developing a predictive model to analyze and estimate the potential severity of product issues based on various internal factors. By leveraging data-driven techniques, the aim is to enhance decision-making and product management strategies.

---

## 🧾 Dataset Overview

The dataset contains various features related to product issues, including:
- Issue type
- Product line
- Issue priority
- Reporter experience
- Time to resolution
- Issue category

---

## 📊 Methodology

### 1. **Data Preprocessing**
- Imported dataset and examined structure
- Handled missing values and outliers
- Converted categorical variables into factors
- Normalized numeric variables

### 2. **Exploratory Data Analysis (EDA)**
- Used `ggplot2` for visual analysis
- Explored class distribution of issue consequences
- Examined correlations and feature importance

### 3. **Model Development**
Models built using training/testing split:
- Logistic Regression
- Decision Tree
- Random Forest
- Gradient Boosting (XGBoost)

Evaluated using:
- Accuracy
- ROC-AUC
- Confusion Matrix

---

## 🧠 Feature Engineering

- Created dummy variables for categorical features
- Engineered features like:
  - `resolution_time_category` (e.g., fast, moderate, slow)
  - `reporter_experience_level` (e.g., novice, expert)

---

## 🔍 Model Evaluation

| Model               | Accuracy | ROC-AUC |
|--------------------|----------|---------|
| Logistic Regression| 0.81     | 0.79    |
| Decision Tree      | 0.78     | 0.76    |
| Random Forest      | 0.85     | 0.87    |
| XGBoost            | 0.89     | 0.91    |

- **XGBoost** outperformed other models across metrics
- Feature importance showed `issue_priority`, `product_line`, and `resolution_time` were most predictive

---

## ✔️ Assumptions & Checks

- No high multicollinearity (VIF < 5)
- Class imbalance was handled with SMOTE
- ROC curves plotted for each model
- Cross-validation used to ensure model robustness

---

## 📈 Visualizations

- Distribution plots for issue types and severity
- Correlation heatmaps
- Feature importance plots from Random Forest and XGBoost
- ROC curves for model comparison

---

## 🧪 Tools Used

- **R**, **RStudio**
- Packages:
  - `tidyverse`, `caret`, `xgboost`, `randomForest`, `rpart`, `pROC`, `ROSE`, `ggplot2`

---

## 📌 Conclusion

The XGBoost model provided the best performance and can be used to predict issue consequences effectively. This model enables early identification of critical product issues, aiding in faster resolution and strategic planning.



