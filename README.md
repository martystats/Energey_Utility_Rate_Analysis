# ⚡ Energy Utility Rate Analysis — EDA + Regression Modeling  

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data--Analysis-green)
![Matplotlib](https://img.shields.io/badge/Visualization-Matplotlib-yellow)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine--Learning-orange)
![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-red)
![GitHub](https://img.shields.io/badge/Version-Control-GitHub-lightgrey)

---

## 📘 Project Overview  
This project explores **energy utility rate data** to analyze and predict residential electricity prices across U.S. states.  
It demonstrates a complete end-to-end **data science workflow**, covering **data cleaning**, **exploratory data analysis (EDA)**, **feature encoding**, **model training**, and **evaluation** using regression algorithms.

The analysis compares rates for **commercial**, **industrial**, and **residential** customers and identifies key patterns that influence pricing across utilities, ownership types, and service types.

---

## 🔍 Key Steps  

### 1. Data Cleaning  
- Removed missing or zero rate values.  
- Standardized column formats and ensured correct data types.  
- Reinforced categorical identifiers (`zip`, `eiaid`, `state`, `utility_name`, etc.) as string types.  
- Verified numerical consistency for rate columns.

### 2. Exploratory Data Analysis (EDA)  
- Generated descriptive statistics for all rate types.  
- Visualized **distributions** (histograms & boxplots) for commercial, industrial, and residential rates.  
- Compared **average rates by ownership and service type**.  
- Computed a **correlation heatmap** among numerical variables (`comm_rate`, `ind_rate`, `res_rate`).

### 3. Insights & Interpretation  
- Identified the **top 5 and bottom 5 states** by average residential electricity rate.  
- Found that **Hawaii (HI)** and **Alaska (AK)** consistently report the highest rates.  
- Discovered **strong correlations** (0.88–0.93) among rate categories.  
- Visualized group trends using comparative bar charts.

### 4. Predictive Modeling (Advanced)  
- Trained and compared four regression models:  
  - **Linear Regression**  
  - **Decision Tree Regressor**  
  - **Random Forest Regressor**  
  - **Gradient Boosting Regressor**  
- Evaluated model accuracy using **Mean Squared Error (MSE)** and **R² Score**.  
- Random Forest and Decision Tree achieved the best performance (R² ≈ 1.00).

### 5. Feature Importance  
- Determined that `comm_rate` and `ind_rate` were the strongest predictors of `res_rate`.  
- Visualized feature importances using side-by-side bar charts for both **Random Forest** and **Gradient Boosting** models.

### 6. Model Export & Deployment Preparation  
- Saved final model as: **`best_regression_model.pkl`**  
- Exported predictions as: **`model_predictions.csv`**  
- Packaged all deliverables (CSV, PKL, Notebook, README) into one GitHub-ready folder for deployment and documentation.

---

## 📊 Results Summary  

| Metric | Best Model | MSE | R² Score |
|:-------|:------------|:----|:---------|
| Random Forest | 0.0000 | **1.00** |
| Decision Tree | 0.0000 | **1.00** |
| Gradient Boosting | 0.0001 | **0.98** |
| Linear Regression | 0.0006 | **0.88** |

✅ The **very low MSE** and **high R²** confirm exceptional model accuracy.  
✅ Predicted residential rates closely match actual outcomes.  
✅ Strong correlation indicates high interdependence between commercial, industrial, and residential pricing trends.

---

## 🧾 Deliverables  

| File | Description |
|:------|:-------------|
| `iou_zipcodes_2023.csv` | Cleaned dataset used for modeling |
| `model_predictions.csv` | Saved predictions for verification |
| `best_regression_model.pkl` | Trained regression model |
| `mynewnotebook19.ipynb` | Full analysis notebook |
| `README.md` | Project documentation |

---

## 🧠 Tools & Technologies  
- **Python 3.10**  
- **Pandas, NumPy** — Data cleaning & manipulation  
- **Matplotlib, Seaborn** — Visualization  
- **Scikit-learn** — Machine Learning & Model Evaluation  
- **Jupyter Notebook** — Interactive analysis  
- **Git & GitHub** — Version control and portfolio management  

---

## 👤 Author  
**Martin Ude**  
GitHub: [martystats](https://github.com/martystats)  
📅 *Project Completed: October 2025*

---

## 🏁 Summary  
This project demonstrates a strong ability to handle **real-world energy pricing data**, from cleaning and exploratory analysis to **machine learning modeling** and **deployment packaging**.  
It highlights analytical depth, technical rigor, and professional documentation ready for inclusion in a data science portfolio.

---
