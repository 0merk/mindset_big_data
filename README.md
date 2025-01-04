# House Price Prediction

### **Objective**
Develop a system to predict house prices using three regression models: Linear Regression, Random Forest Regression, and Support Vector Regression (SVR).

---

### **Methodology**

#### Data Loading and Exploration
- **Data Exploration:**
  - Loaded the `house.csv` dataset into a pandas DataFrame (`df`).
  - Performed basic data analysis using `df.head()`, `df.tail()`, `df.shape`, `df.info()`, and `df.describe()`.
- **Visualization:**
  - Plotted correlations using a heatmap (`seaborn.heatmap`).
  - Detected outliers with box plots for each feature.
- **Outlier Removal:** 
  - Applied the IQR method to clean the `price` column.

#### Linear Regression Model
- **Data Preparation:**
  - Separated features (`X`) and target variable (`y`).
  - Scaled features using `StandardScaler`.
  - Split the dataset into training and testing sets with `train_test_split`.
- **Model Training:** Trained a Linear Regression model.
- **Model Evaluation:**
  - Calculated Mean Squared Error (MSE) and R-squared (R²).
  - Visualized predictions vs. actual values using a scatter plot.
  - Analyzed residuals and calculated adjusted R-squared.

#### Random Forest Regression Model
- **Model Training:** Built a Random Forest Regression model.  
- **Model Evaluation:**  
  - Computed R-squared error.
  - Plotted actual vs. predicted prices with a line plot.

#### Support Vector Regression (SVR) Model
- **Data Preparation:** Similar to the Linear Regression process.
- **Model Training:** Trained an SVR model with a linear kernel.
- **Model Evaluation:**  
  - Plotted actual vs. predicted values.  
  - Analyzed residuals.  
  - Displayed feature coefficients.

---

### **Findings**
- Identified key preprocessing steps like outlier removal and feature scaling as critical for model performance.  
- Demonstrated the strengths and weaknesses of each regression model:
  - **Linear Regression:** Simple and interpretable but may lack flexibility.  
  - **Random Forest:** Non-linear and robust, providing strong performance.  
  - **SVR:** Effective for small datasets with linear relationships but computationally intensive.

---

### **Tools Used**
- **Python Libraries:** `Pandas`, `Matplotlib`, `Seaborn`, `Scikit-learn`.
