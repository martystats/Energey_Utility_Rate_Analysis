# ⚡ Energy Utility Rates Analysis — EDA + Regression Modeling

## 📘 Project Overview  
This project investigates **U.S. Electric Utility Rates** by analyzing commercial (`comm_rate`), industrial (`ind_rate`), and residential (`res_rate`) electricity pricing data across different states, ownership types, and service structures.  
The goal is to perform a **complete data-science workflow** — from **cleaning and exploratory data analysis (EDA)** to **predictive modeling** using multiple regression algorithms.

The study identifies rate disparities across utilities, highlights factors influencing residential rates, and applies regression models to predict `res_rate` based on other variables.

---

## 🧭 Key Steps  

### 🧹 1. Data Cleaning  
- Reinforced column data types (`zip`, `eiaid` → string).  
- Verified no missing or duplicate records.  
- Standardized string formats for categorical columns.  

### 📊 2. Exploratory Data Analysis (EDA)  
- Generated numerical and categorical summary statistics.  
- Visualized rate distributions (histograms, boxplots).  
- Compared rates by **Ownership Type** and **Service Type**.  
- Computed correlation matrix among rate variables.  
- Identified top and bottom five states by average residential rate.

### 🧠 3. Modeling  
- Defined `res_rate` as target and trained multiple regressors:  
  - **Linear Regression**  
  - **Decision Tree Regressor**  
  - **Random Forest Regressor**  
  - **Gradient Boosting Regressor**  
- Evaluated models using **R²** and **Mean Squared Error (MSE)** metrics.  
- Visualized **Actual vs Predicted Residential Rates** for the best model.  

### 🔍 4. Feature Importance  
- Assessed predictor significance using **Random Forest** and **Gradient Boosting** importance scores.  
- Found `comm_rate` to be the strongest determinant of `res_rate`.  

### 💾 5. Packaging  
All deliverables have been saved and uploaded for reproducibility and external access.

---

## 🧩 Results Summary  

| Model | MSE | R² Score |
|:--|--:|--:|
| Decision Tree | 0.00 | 1.00 |
| Random Forest | 0.00 | 1.00 |
| Gradient Boosting | 0.00 | 0.98 |
| Linear Regression | 0.00 | 0.88 |

**Key Insight:**  
- Extremely low MSE and near-perfect R² (~0.9997) indicate **exceptional predictive performance**.  
- Residential rate trends are primarily influenced by commercial and industrial rates, with minimal contribution from ownership and service type.

---

## 📁 Deliverables  

| File | Description |
|:--|:--|
| `iou_zipcodes_2023.csv` | Cleaned dataset used for analysis |
| `mynewnotebook19.ipynb` | Jupyter notebook containing full workflow |
| `best_regression_model.pkl` | Saved best-performing regression model |
| `model_predictions.csv` | Predicted values for residential electricity rates |
| `README.md` | Project documentation and GitHub summary |

---

## 🧰 Tools & Libraries  
- Python 3.10  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-Learn  
- Joblib  
- Jupyter Notebook  

---

## 🚀 Author  
**Martin Ude**  
Data Science Portfolio — [@martystats](https://github.com/martystats)  
📅 *Completed: October 2025*  

---

### 🏁 Summary
This project successfully demonstrates a full **end-to-end machine-learning pipeline** on real-world utility rate data — from data cleaning and visualization to model training, evaluation, and deployment-ready packaging.  
It is a strong example of **predictive analytics applied to energy economics** and is fully reproducible for review or extension.

---

