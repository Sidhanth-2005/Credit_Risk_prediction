# 🧠 Credit Default Prediction using Machine Learning  
[![Python](https://img.shields.io/badge/Python-3.10-blue.svg)](https://www.python.org/)  
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Model-orange.svg)](https://scikit-learn.org/)  
[![XGBoost](https://img.shields.io/badge/XGBoost-0.9+-green.svg)](https://xgboost.readthedocs.io/)  
[![Google Colab](https://img.shields.io/badge/Google-Colab-yellow.svg)](https://colab.research.google.com/)  
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

---

## 📘 Overview  
This project predicts **the probability of a person defaulting on a loan within two years** using credit history data.  
It uses machine learning classification models such as **Logistic Regression**, **Random Forest**, and **XGBoost** to identify high-risk borrowers.

---

## 🧩 Dataset Description  
Each row represents a person with their financial and demographic information.  

| Feature | Description |
|----------|--------------|
| `SeriousDlqin2yrs` | Target variable — 1 if person defaulted, 0 otherwise |
| `RevolvingUtilizationOfUnsecuredLines` | Ratio of credit card balance to total credit limit |
| `age` | Age of the borrower |
| `NumberOfTime30-59DaysPastDueNotWorse` | Times borrower was 30–59 days late |
| `DebtRatio` | Debt payments to monthly income ratio |
| `MonthlyIncome` | Monthly income |
| `NumberOfOpenCreditLinesAndLoans` | Open loans and credit lines |
| `NumberOfTimes90DaysLate` | Times borrower was 90+ days late |
| `NumberRealEstateLoansOrLines` | Real estate loans count |
| `NumberOfTime60-89DaysPastDueNotWorse` | Times borrower was 60–89 days late |
| `NumberOfDependents` | Number of dependents |

---

## ⚙️ Project Workflow  
1. **Data Preprocessing**  
   - Removed irrelevant columns (`Unnamed: 0`)  
   - Handled missing values in `MonthlyIncome` and `NumberOfDependents`  
   - Split data into features (`X_train`) and target (`y_train`)

2. **Model Training**  
   - Algorithms used:
     - Logistic Regression  
     - Random Forest  
     - XGBoost  

3. **Model Evaluation**  
   - Evaluated models using:  
     - **Accuracy**  
     - **ROC-AUC**  
     - **Precision, Recall, F1-score**

---

## 📊 Results  

| Model | ROC-AUC | Accuracy |
|--------|----------|-----------|
| **XGBoost** | 0.5945 | 0.9389 |
| **Random Forest** | 0.5917 | 0.9364 |

**Precision:** 0.5942  
**Recall:** 0.1984  
**F1-Score:** 0.2974  

> ⚠️ The dataset is **imbalanced**, meaning most people did *not* default — so accuracy alone can be misleading.

---

## 🧠 Insights  
- High accuracy (~93%) doesn’t mean the model performs well due to imbalance.  
- ROC-AUC gives a better sense of true performance.  
- Improvement can be achieved with techniques like **SMOTE**, **class weighting**, or **resampling**.  

---

## 🚀 Future Improvements  
✅ Apply SMOTE or undersampling for balancing.  
✅ Use hyperparameter tuning with GridSearchCV.  
✅ Try advanced models (LightGBM, CatBoost, Neural Nets).  

---

## 🛠️ Tech Stack  
- **Language:** Python 🐍  
- **Libraries:** Scikit-Learn, XGBoost, Pandas, NumPy, Matplotlib  
- **Environment:** Google Colab  
- **Version Control:** GitHub  

---


## ✍️ Author  
**Sidhanth**  
💡 *Machine Learning Enthusiast | Data-Driven Problem Solver*  
📫 Connect with me on [LinkedIn](https://www.linkedin.com/)  

---

## 📜 License  
This project is licensed under the **MIT License** – feel free to use and modify with attribution.

