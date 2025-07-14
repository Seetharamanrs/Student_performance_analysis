# Student Performance Analytics 

This project analyzes student academic performance using data from the UCI Machine Learning Repository. It includes:

- Data cleaning and EDA
- Visualizations
- Random Forest Regression
- Logistic Regression
---
## Structure

- `data/`: Raw datasets (`student-mat.csv`, `student-por.csv`)
- `notebooks/`: Jupyter notebooks with code
- `visuals/`: Saved plots and charts
- `requirements.txt`: Python packages needed

## Dataset Summary 
- **Total Samples:** 649
- **Features:** 33
- **Target Variable:** `G3` (Final Grade: 0–20)
No missing values found in dataset 
---

## Key Insights

- The most important feature for predicting `G3` (final grade) is `G2` (second period grade).
- This suggests that students who score well in `G2`(second period grade) are highly likely to score similarly in `G3`(final grade).
- Features like **study time**, **parental education**(especially the mother's), and **alcohol consumption**(weekdays and weekends) also showed varying degrees of correlation with academic performance.
- These insights can help identify at-risk students early for timely academic support.
- All relevant plots and graphs can be found in the `visuals/` directory.

---

##  Models Used

### 1. Random Forest Regressor
- **Approach:** Converted final grade into binary (Pass/Fail) for classification.
- **Hyperparameter Tuning:** Used `GridSearchCV` to optimize performance.
- **Accuracy:** ~92.3% on test data.
- **Top Feature:** `G2` (Second period grade)`

### 2. Logistic Regression
- Applied for binary classification (pass/fail) using the same features
- Also validated the high predictive power of G2 (second period grade)
- Attempted classification based on grade performance buckets

---

## Requirements

See `requirements.txt` to install dependencies:
## How to Run

```bash
pip install -r requirements.txt