# 🧬 TCGA-BRCA Survival Analysis & Prediction

A complete end-to-end **survival analysis and machine learning pipeline** built on TCGA Breast Cancer (BRCA) clinical data.  
This project combines **statistical survival modeling + predictive ML + interpretability** to derive meaningful clinical insights.

---

## 🚀 Overview

This project analyzes **1,084 breast cancer patients** to:

- Understand survival patterns
- Identify key risk factors
- Predict 5-year survival outcomes
- Stratify patients into risk groups

It integrates:
- 📊 Survival Analysis (Kaplan-Meier, Cox PH)
- 🤖 Machine Learning Models
- 🔍 Model Explainability
- 📈 Clinical Visualization

---

## 📂 Dataset

- Source: TCGA BRCA (cBioPortal)
- Patients: **1,084**
- Final processed: **1,071**
- Features engineered: **80**

---

## ⚙️ Pipeline Highlights

### 1. Data Preprocessing
- Cleaned missing/invalid survival values
- Encoded categorical variables
- Removed constant & collinear features

---

### 2. Survival Analysis

**Kaplan-Meier Analysis**
- Significant survival differences across:
  - Tumor subtype *(p = 0.024)*
  - Tumor stage *(p < 0.001)*
  - Radiation therapy *(p = 0.003)*

**Cox Proportional Hazards Model**
- Identified key risk factors:
  - Cancer status (HR ≈ 1.86)
  - Age (HR ≈ 1.01 per year)
  - Tumor recurrence indicators

---

### 3. Machine Learning Models

Built a **5-year survival classifier** using:

- Logistic Regression
- Random Forest ✅ (Best)
- Gradient Boosting
- XGBoost
- Neural Network (MLP)

---

## 🏆 Results

| Metric        | Best Model (Random Forest) |
|--------------|--------------------------|
| ROC-AUC      | **0.834 ± 0.054**        |
| F1 Score     | **0.832 ± 0.043**        |
| PR-AUC       | **0.933 ± 0.025**        |
| Accuracy     | **0.773 ± 0.054**        |

---

## 📊 Key Insights

- Higher tumor stage → significantly worse survival  
- Recurrence strongly increases risk  
- Age has a consistent but moderate effect  
- Clear separation between **high-risk vs low-risk patients**

---

## 📉 Visualizations

The pipeline generates:

- Kaplan-Meier survival curves  
- Cox hazard forest plots  
- ROC & Precision-Recall curves  
- Confusion matrices  
- Risk stratification plots  
- Feature importance plots  

---

## 🔍 Explainability

- SHAP initially attempted  
- Fallback: **Permutation Importance**
- Identified most influential clinical features affecting survival prediction

---

## 🛠️ Tech Stack

- Python  
- Pandas, NumPy  
- Lifelines (Survival Analysis)  
- Scikit-learn  
- XGBoost  
- Matplotlib / Seaborn  

---

## 📌 Key Strengths of This Project

- End-to-end pipeline (raw data → insights → prediction)
- Combines **statistics + ML + interpretability**
- Handles **real-world clinical challenges**:
  - Censored data
  - Class imbalance
  - Feature engineering
- Strong evaluation using cross-validation

---

## 📎 Output

All results include:
- Cleaned dataset  
- Model comparison metrics  
- Risk scores  
- High-quality plots  

---

## 💡 Future Improvements

- Deep survival models (DeepSurv)
- Better handling of censored data in ML
- Hyperparameter tuning
- External validation dataset

---

## 👩‍💻 Author

**Sneha Suresh**  
Aspiring Bioinformatics & Data Science Professional  

---

## ⭐ Why This Project Matters

This project demonstrates the ability to:
- Work with **real biomedical datasets**
- Apply **advanced statistical techniques**
- Build **production-level ML pipelines**
- Translate data into **actionable insights**
