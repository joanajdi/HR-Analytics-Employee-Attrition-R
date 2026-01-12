# HR Analytics: Employee Attrition Prediction  

This project aims to **identify the main factors influencing employee attrition** and develop a **predictive model** to anticipate turnover risk.  
The dataset used is **IBM HR Analytics Employee Attrition & Performance** (publicly available on Kaggle).

---

## Objective

To go beyond mere prediction and extract **actionable business insights** that help HR departments design strategic retention policies.

---

## Dataset

- **Source:** IBM HR Analytics Employee Attrition & Performance (Kaggle)  
- **Observations:** 1,470 employees  
- **Variables:** 35 demographic, professional, and satisfaction metrics  
- **Target:** `Attrition` (Yes = Employee left, No = Stayed)

---

## Methodology

1. **Exploratory Data Analysis (EDA)**
   - Distribution analysis, correlation mapping, and feature relevance.
2. **Data Pre-processing**
   - Cleaning, one‑hot encoding, handling collinearity, and class balancing (ROSE).
3. **Modeling**
   - Logistic Regression and Random Forest comparison.
4. **Evaluation Metrics**
   - Accuracy, Recall (Sensitivity), and Specificity.
5. **Feature Importance Analysis**
   - Identification of top variables influencing employee attrition.

---

## Results Summary

| Metric | Logistic Regression | Random Forest |
|--------|---------------------|---------------|
| Accuracy | 72.8% | **74.1%** |
| Recall (Sensitivity) | **73.2%** | 70.4% |
| Specificity | — | **74.9%** |

**Random Forest** achieved a better trade‑off between detection and precision, serving as the final deployed model.

---

## Key Insights

1. **Job Role matters most** – Sales Representatives are at highest risk, while Directors show high stability.  
2. **OverTime** is a critical trigger – work overload strongly increases attrition probability.  
3. **Stock Options** have a clear retention effect – long-term ownership improves stability more than salary increases.  
4. **Early departure risk** peaks within the first 2 years of employment.

---

## Recommendations for HR

1. Review incentives and workload in Sales roles.  
2. Implement controls and compensations for overtime.  
3. Strengthen career development and “onboarding” mentoring.  
4. Maintain periodic predictive monitoring with Random Forest to flag at‑risk employees.

---

## Technologies

**R**, **ggplot2**, **dplyr**, **corrplot**, **ROSE**, **randomForest**, **caret**, **kableExtra**

---

## Reproducibility

To reproduce the report:

```r
rmarkdown::render("HR_Attrition_Project.Rmd")
```

---

📎 **Full Report (HTML):** [link-to-your-HTML-after-upload]

👩💻 **Author:** https://www.linkedin.com/in/joanainacio000/
