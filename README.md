# Data_Analysis_of_House_Pricing_Dataset
Here I analyzed a House Price Dataset of King County in USA for IBM Data Science Professional Certification. The dataset is also available in the kaggle.

## Link for the Kaggle dataset of King County in USA
[![Kaggle](https://shields.io)]([https://kaggle.com](https://www.kaggle.com/datasets/harlfoxem/housesalesprediction))

## Used tools
<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white"/>
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
  <img src="https://img.shields.io/badge/Scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white"/>
  <img src="https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/IBM-052FAD?style=for-the-badge&logo=ibm&logoColor=white"/>
</p>

---
## 📋 Project Overview

This repository contains a **data analytics and machine learning capstone project** completed as part of the IBM Data Science Professional Certificate programm. It performs a comprehensive end-to-end analytical workflow on the **King County, USA house sales dataset** — covering Exploratory Data Analysis (EDA), data wrangling, statistical visualization, predictive model development and model refinement using regression techniques.

The project demonstrates the full data science pipeline: from raw data ingestion and cleaning, through visual correlation analysis, to model training, evaluation, and regularisation — resulting in quantified predictive performance metrics for house price estimation.

---

## 🎯 Analytical Objectives

The project addresses 10 structured analytical questions (`Q1`–`Q10`) that progressively deepen the analytical complexity:

| Question | Focus Area | Technique |
|:---|:---|:---|
| Q1 | Dataset structure & types | `df.dtypes`, `df.describe()` |
| Q2 | Data cleaning | Drop irrelevant columns (`id`, `Unnamed: 0`), null inspection |
| Q3 | Unique value distributions | `.value_counts().to_frame()` — floors, bedrooms, waterfront |
| Q4 | Waterfront impact on price | Box plot — price vs waterfront attribute |
| Q5 | Price vs square footage | Regression plot (`sns.regplot`) — `sqft_above` vs `price` |
| Q6 | Simple linear regression | `LinearRegression` on `sqft_living` → R² score |
| Q7 | Multiple linear regression | Multi-feature model — floors, waterfront,lat ,bedrooms ,sqft_basement ,view ,bathrooms,sqft_living15,sqft_above,grade,sqft_living |
| Q8 | Scikit-learn Pipeline | `StandardScaler` + `PolynomialFeatures` + `LinearRegression` via `Pipeline` |
| Q9 | Ridge Regression | `Ridge(alpha=0.1)` — regularised model fit and evaluation |
| Q10 | Regularisation comparison | Second-order polynomial + Ridge → R² improvement quantified |

---
