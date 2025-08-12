# Air Quality Index Prediction

## 📌 Overview

This project predicts the **Air Quality Index (AQI)** for Delhi using historical air quality data from Kaggle.  
The focus was on **feature engineering**, **polynomial regression modeling**, and **model evaluation** to achieve a high predictive performance.

Dataset source: [Delhi Air Quality Dataset – Kaggle](https://www.kaggle.com/datasets/kunshbhatia/delhi-air-quality-dataset/data)

---

## 🔍 Project Workflow

1. **Data Loading**  
   - Imported dataset from Kaggle.  
   - Checked for missing values and performed basic exploratory data analysis (EDA).  

2. **Feature Engineering**  
   - Dropped weakly correlated features with AQI to reduce noise.  
   - Created a **Polynomial Features** set (degree = 2) for non-linear relationships.  
   - Applied **Standard Scaling** to normalize feature ranges.  

3. **Modeling**  
   - Used a **Pipeline** containing:  
     1. `PolynomialFeatures(degree=2)`  
     2. `StandardScaler()`  
     3. `LinearRegression()`  

4. **Evaluation Metrics**  
   - **R² Score:** 0.934  
   - **MSE:** 856.91  
   - **RMSE:** 29.27  
   - **MAE:** 21.11  

5. **Error Analysis**  
   - Residuals vs Predicted Plot – to check if errors are randomly distributed.  
   - Predicted vs Actual AQI Plot – to visualize how well the model fits.  

---

## 📊 Results

The model achieved strong predictive performance:  

| Metric      | Value   |  
|-------------|---------|  
| **R²**      | 0.934   |  
| **MSE**     | 856.91  |  
| **RMSE**    | 29.27   |  
| **MAE**     | 21.11   |   

Learning curve analysis shows no major signs of overfitting, with training and validation scores converging closely.  

---

## 📈 Plots Included

- **Residual Error vs Predicted**  
- **Predicted vs Actual**  
- **Learning Curve**  

---

## 🛠️ Tech Stack

- **Python** (Pandas, NumPy, Matplotlib, Seaborn, scikit-learn)  
- **VS Code with Jupyter Extension** for experimentation  
- **scikit-learn Pipelines** for clean model workflow  

---
