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
- This suggests that students who score well in `G2` are highly likely to score similarly in `G3`.
- Features like **study time**, **parental education**, and **alcohol consumption** also showed varying degrees of correlation with academic performance.
- All relevant plots and graphs can be found in the `visuals/` directory.

---

##  Models Used

### 1. Random Forest Regressor
- **Metric:** R² score, Mean Squared Error
- **Result:** High importance given to `G2`

### 2. Logistic Regression
- Attempted classification based on grade performance buckets

---

## Requirements

See `requirements.txt` to install dependencies:
## How to Run

```bash
pip install -r requirements.txt