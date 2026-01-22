# 📊 Simple Linear Regression: Skill Count vs Salary

## 🔍 Overview  
This project analyzes the **association between skill count and salary (LPA)** using **Simple Linear Regression (OLS)**.  
The goal is **statistical association**, not causal inference or production-level prediction.

---

## 📁 Dataset  
The dataset contains two numerical variables:

- **`skill_count`** – Number of skills possessed  
- **`salary_lpa`** – Annual salary in Lakhs Per Annum  

No missing values or categorical features are present.

---

## 🧠 Methodology  
- Simple Linear Regression (OLS)  
- Train–test split for validation  
- Model evaluation using **R²** and **RMSE**

Regression equation:

```
salary_lpa = β₀ + β₁ × skill_count + ε
```

---

## 🔍 Model Diagnostics  
The following diagnostic checks were performed:

- **📉 Residual Analysis**:  
  Standardized residuals vs standardized predicted values were plotted to assess homoscedasticity.

- **🚨 Outlier Detection**:  
  Z-score method applied to identify extreme salary values (|Z| > 3).

- **📈 Autocorrelation Check**:  
  Durbin–Watson statistic indicated positive autocorrelation, suggesting partial violation of OLS assumptions.

---

## 📌 Results  
- ✅ Strong positive linear association between skill count and salary  
- 📈 High explanatory power (R² ≈ 0.98)  
- 📉 Low prediction error on validation data  

⚠️ Due to autocorrelation, standard errors and p-values should be interpreted with caution.

---

## ⚠️ Limitations  
- Single predictor model  
- Potential omitted variable bias  
- Autocorrelation affects inference reliability  
- Results indicate association, not causation

---

## 🔮 Future Work  
- Use **Newey–West standard errors** for robust inference  
- Extend to multivariate regression with experience and role-based variables  
- Apply formal diagnostic tests for heteroscedasticity and autocorrelation  
- Explore nonlinear and quantile regression models

---

## 🛠️ Tools Used  
Python, Pandas, NumPy, Matplotlib, Scikit-learn, Statsmodels

---

## 🧾 Final Note  
This is a **clean academic-level regression project** with proper diagnostics.  
It demonstrates understanding of **OLS assumptions**, not just model fitting.
