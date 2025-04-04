# Housing-Investment-Prediction

# Multiple Linear Regression (MLR) Projects

## Project 1: House Price Prediction using Backward Elimination

### Overview

This project focuses on predicting house prices using multiple linear regression (MLR) with backward elimination to identify statistically significant features. The dataset includes various attributes like square footage, number of bedrooms, bathrooms, and location details.

### Key Steps

1. **Data Preprocessing**:

   - Dropped irrelevant columns (`id`, `date`).
   - Checked for missing values and categorical data.
2. **Exploratory Data Analysis (EDA)**:

   - Visualized relationships between features using `seaborn.pairplot`.
3. **Model Training**:

   - Split data into training and testing sets.
   - Trained a linear regression model.
4. **Backward Elimination**:

   - Used `statsmodels.OLS` to iteratively remove insignificant features (p-value > 0.05).
   - Evaluated model performance using R-squared and adjusted R-squared.

---

## Project 2: Investment Prediction with MLR

### Overview

This project predicts investment outcomes using multiple linear regression. The dataset includes features like R&D spend, administration costs, and marketing spend across regions.

### Key Steps

1. **Data Preprocessing**:

   - Encoded categorical variables (e.g., region) using `pd.get_dummies`.
   - Appended a constant term for the intercept.
2. **Model Training**:

   - Split data into 80% training and 20% testing sets.
   - Trained a linear regression model and predicted test values.
3. **Feature Selection**:

   - Applied backward elimination manually by inspecting p-values from OLS summaries.
   - Simplified the model iteratively to retain only significant features.
4. **Performance Metrics**:

   - Calculated bias (training score) and variance (testing score) to assess overfitting.

---

## How to Use

1. Clone the repository:
   ```bash
   git clone [repository_url]
   ```
2. Install dependencies:
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn statsmodels
   ```
3. Run the Jupyter notebook (`MLR-Housing.ipynb`) or Python script (`MLR-Investment.py`).

## Dependencies

- Python 3.x
- Libraries: `numpy`, `pandas`, `matplotlib`, `seaborn`, `scikit-learn`, `statsmodels`
