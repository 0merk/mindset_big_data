# mindset_big_data
# House Price Prediction

This project implements a house price prediction system using three regression models: **Linear Regression**, **Random Forest Regression**, and **Support Vector Regression (SVR)**. The analysis and modeling are structured into the following sections:

---

## 1. Data Loading and Exploration
- **Libraries Used:** `pandas`, `matplotlib`, `seaborn`, `scikit-learn`
- **Dataset:** `house.csv`, loaded into a pandas DataFrame (`df`).
- **Exploratory Data Analysis (EDA):**
  - Basic dataset information using `df.head()`, `df.tail()`, `df.shape`, `df.info()`, and `df.describe()`.
  - **Correlation Analysis:** Heatmap visualization using `seaborn.heatmap`.
  - **Outlier Detection:** Box plots for each feature.
  - **Outlier Removal:** IQR method applied to the `price` column.

---

## 2. Linear Regression Model
- **Data Preparation:**
  - Separated features (`X`) and target variable (`y`).
  - Scaled features using `StandardScaler`.
  - Split dataset into training and testing sets using `train_test_split`.
- **Model Training:** Linear Regression model trained on the processed data.
- **Model Evaluation:**
  - **Metrics:** Mean Squared Error (MSE) and R-squared (R²).
  - **Visualizations:**
    - Scatter plot of predictions vs. actual values.
    - Residual analysis and adjusted R-squared calculation.

---

## 3. Random Forest Regression Model
- **Model Training:** Random Forest Regression model trained on the dataset.
- **Model Evaluation:**
  - **Metrics:** R-squared error.
  - **Visualizations:** Line plot comparing actual and predicted prices.

---

## 4. Support Vector Regression (SVR) Model
- **Data Preparation:** Similar process to Linear Regression.
- **Model Training:** SVR model trained using a linear kernel.
- **Model Evaluation:**
  - **Visualizations:**
    - Scatter plot of actual vs. predicted values.
    - Residual plot.
    - Display of feature coefficients.

---

## Key Insights
- Compared the performance of three regression models for house price prediction.
- Highlighted the importance of data preprocessing, including outlier removal and feature scaling.
- Provided clear visualizations for model evaluation and interpretability.

---

Feel free to explore the code and analysis for each model in the repository. Contributions and suggestions are welcome!
