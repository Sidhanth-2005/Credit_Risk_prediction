# 🧠 Credit Default Prediction using Machine Learning  
[![Python](https://img.shields.io/badge/Python-3.10-blue.svg)](https://www.python.org/)  
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Model-orange.svg)](https://scikit-learn.org/)  
[![XGBoost](https://img.shields.io/badge/XGBoost-0.9+-green.svg)](https://xgboost.readthedocs.io/)  
[![Kaggle](https://img.shields.io/badge/Kaggle-Notebook-blue.svg)](https://www.kaggle.com/)  
[![Google Colab](https://img.shields.io/badge/Google-Colab-yellow.svg)](https://colab.research.google.com/)  
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

---

## 🌟 Project Highlights  
This project focuses on **predicting the likelihood of credit default** using financial and demographic data from the **Kaggle "Give Me Some Credit" competition**.  
It includes **data preprocessing, model building, evaluation, and interpretation** — first implemented in **Kaggle Notebooks**, then refined and documented in **Google Colab** for GitHub.

**Key Features:**  
- End-to-end ML workflow from data cleaning to model prediction  
- Comparison of **Logistic Regression, Random Forest, and XGBoost**  
- ROC-AUC, Precision, Recall, and F1-score evaluation  
- Clear handling of **imbalanced dataset issues**  
- Ready-to-run Colab notebook and Kaggle-compatible pipeline  

---

## 📘 Overview  
This project predicts **the probability of a borrower defaulting within two years** based on historical credit behavior.  
It demonstrates how ML models can detect financial risk patterns and assist in responsible lending decisions.

---

## 🧩 Dataset Description  
Dataset source: [Kaggle - Give Me Some Credit](https://www.kaggle.com/c/GiveMeSomeCredit)  

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
   - Split data into `X_train` and `y_train`

2. **Model Training**  
   - Implemented:
     - Logistic Regression  
     - Random Forest  
     - XGBoost  

3. **Model Evaluation**  
   - Metrics used:  
     - **Accuracy**  
     - **ROC-AUC**  
     - **Precision**, **Recall**, **F1-score**

---

## 📊 Results  

| Model | ROC-AUC | Accuracy |
|--------|----------|-----------|
| **XGBoost** | 0.5945 | 0.9389 |
| **Random Forest** | 0.5917 | 0.9364 |

**Precision:** 0.5942  
**Recall:** 0.1984  
**F1-Score:** 0.2974  

> ⚠️ The dataset is **imbalanced** — most people did *not* default, so accuracy alone can be misleading.

---

## 🧠 Insights  
- High accuracy (~93%) is due to class imbalance — not necessarily good prediction of defaulters.  
- ROC-AUC is a better measure of discrimination ability.  
- Performance can be improved with **resampling**, **feature scaling**, and **hyperparameter tuning**.

---

## 🚀 Future Improvements  
✅ Apply SMOTE or undersampling for balancing.  
✅ Use GridSearchCV for parameter tuning.  
✅ Experiment with LightGBM, CatBoost, or deep learning models.  

---

## 🛠️ Tech Stack  
- **Language:** Python 🐍  
- **Libraries:** Scikit-Learn, XGBoost, Pandas, NumPy, Matplotlib  
- **Platforms:** Kaggle Notebooks, Google Colab  
- **Version Control:** GitHub  


---

## ✍️ Author  
**Sidhanth**  
💡 *Machine Learning Enthusiast | Data-Driven Problem Solver*  
📫 Connect with me on [LinkedIn](https://www.linkedin.com/)  

---

## 📜 License  
This project is licensed under the **MIT License** – feel free to use and modify with attribution.
