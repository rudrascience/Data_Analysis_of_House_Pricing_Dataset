# Data_Analysis_of_House_Pricing_Dataset
Here I analyzed a House Price Dataset of King County in USA for IBM Data Science Professional Certification. The dataset is also available in the kaggle.

---
## Link for the Kaggle dataset of King County in USA
[![Kaggle](https://img.shields.io/badge/Kaggle-houseprice-skyblue?style=flat&logo=kaggle&logoColor=white)](https://www.kaggle.com/datasets/harlfoxem/housesalesprediction)
---
## Repository Link
([https://github.com/rudrascience/Data_Analysis_of_House_Pricing_Dataset/blob/main/README.md])

---
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
## 🛠️ Technology Stack

| Technology | Role |
|:---|:---|
| **Python 3.x** | Core language |
| **Jupyter Notebook** | Interactive analysis environment |
| **Pandas** | Data loading, cleaning, transformation, groupby |
| **NumPy** | Numerical operations and array handling |
| **Matplotlib** | Base plotting library |
| **Seaborn** | Statistical visualisation (`regplot`, `boxplot`) |
| **Scikit-learn** | `LinearRegression`, `Ridge`, `Pipeline`, `PolynomialFeatures`, `StandardScaler`, `train_test_split` |

**Notebook composition:**

```
Python / Jupyter cells (EDA + modelling)   ████████████████████  ~80%
Visual evidence                            ████████░░░░░░░░░░░░  ~25%
Markdown documentation                     ██░░░░░░░░░░░░░░░░░░   ~5%
```
## 📊 Dataset Summary

| Attribute | Value |
|:---|:---|
| **Dataset** | King County House Sales (USA) |
| **Source** | IBM Skills Network / Kaggle variant |
| **Records** | ~21,613 house sale transactions |
| **Features** | 21 (bedrooms, bathrooms, sqft_living, sqft_lot, floors, waterfront, view, condition, grade, sqft_above, sqft_basement, yr_built, yr_renovated, zipcode, lat, long, sqft_living15, sqft_lot15) |
| **Target variable** | `price` (house sale price in USD) |
| **Date range** | May 2014 – May 2015 |

---

## 🔬 Modelling Pipeline Detail

```
1. Data Ingestion
   └── pd.read_csv() → DataFrame

2. Data Wrangling
   ├── Drop: ['id', 'Unnamed: 0']
   ├── Null check & removal
   └── dtypes inspection

3. Exploratory Data Analysis
   ├── value_counts() → categorical distributions
   ├── sns.boxplot() → price vs waterfront
   └── sns.regplot() → price vs sqft_above

4. Model Development
   ├── Simple LR:   LinearRegression(sqft_living) → R²
   ├── Multiple LR: LinearRegression(7 features)  → R²
   ├── Pipeline:    StandardScaler + PolynomialFeatures(2) + LR → R²
   └── Ridge:       Ridge(alpha=0.1) + Polynomial(2) → R² (best)

5. Model Refinement
   └── R² score comparison across all 4 models
```

## 📚 Course Context

| Detail | Value |
|:---|:---|
| Course | Data Analysis with Python |
| Provider | IBM / Coursera |
| Certificate | IBM Data Science Professional Certificate |
| Assignment | Final Capstone Lab |
| Dataset | King County House Sales, USA |

---
**👤 Author: [Rudrajit Das](https://github.com/rudrascience)** ·
