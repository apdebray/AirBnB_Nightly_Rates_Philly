# Optimizing Nightly Rates for Airbnb Hosts in Philadelphia

## 📌 Project Overview

This project leverages machine learning techniques to **predict optimal nightly rates** for Airbnb listings in Philadelphia using a real-world dataset containing over **11.5 million data points**. The model is designed to assist hosts in maximizing revenue based on listing characteristics, location, and performance indicators.

The analysis spans **classification models** (to predict Superhost likelihood) and **regression models** (to estimate optimal nightly rates), providing a dual approach to both improve host performance and pricing strategies.

## 🧠 Problem Statement

* **How can Airbnb hosts in Philadelphia optimize their nightly rates for revenue maximization?**
* **What listing characteristics most influence Superhost designation and pricing success?**

Using a rich dataset scraped from Airbnb’s platform, we answer these questions through **feature engineering**, **preprocessing pipelines**, and **model evaluation**.

---

## 📁 Repository Structure

```
apdebray-airbnb_nightly_rates_philly/
│
├── README.md                                ← Project documentation (this file)
├── FinalProjIteration.ipynb                 ← Full EDA, classification & regression notebooks
└── Optimizing-Nightly-Rates...PART1.pptx    ← Final slide presentation summarizing findings
```

---

## 🧰 Tools & Technologies

| Category          | Tools & Libraries                   |
| ----------------- | ----------------------------------- |
| **Languages**     | Python                              |
| **ML Libraries**  | `scikit-learn`, `XGBoost`           |
| **Visualization** | `matplotlib`, `seaborn`             |
| **Data Handling** | `pandas`, `numpy`                   |
| **Deployment**    | Jupyter (Google Colab), CSV outputs |

---

## 🔍 Project Highlights

### 📈 Regression Modeling (Nightly Rate Prediction)

* **Target Variable**: `Nightly Rate`

* **Models Evaluated**:

  * `RandomForestRegressor`
  * `GradientBoostingRegressor`
  * `XGBoostRegressor`

* **Top Performer**: **Random Forest**

* **Best Metrics**:

  * **MAE**: 103.37
  * **RMSE**: 182.88
  * **R² Score**: 0.77

* **Key Features**: Listing type, number of beds, amenities, host location, and guest ratings.

### 🤝 Classification Modeling (Superhost Prediction)

* **Target Variable**: `host_is_superhost_in_period`

* **Models Evaluated**:

  * `RandomForestClassifier`
  * `GradientBoostingClassifier`
  * `XGBoostClassifier`

* **Top Performer**: **XGBoost**

* **Best Metrics**:

  * **Accuracy**: 0.98
  * **Precision**: 0.94
  * **Recall**: 0.96
  * **F1-Score**: 0.95
  * **ROC AUC**: 0.99

* **Feature Importance**: Price, availability, location, prior performance metrics

### 🧼 Data Preprocessing Pipeline

* **Missing value imputation**
* **Column dropping for data leakage prevention**
* **Standard scaling of numerical features**
* **One-hot encoding of categorical variables**
* **Train-test split stratification for fair classification**

---

## 📊 Presentation Summary

**Optimizing-Nightly-Rates-for-Airbnb-PhiladelphiaPART1.pptx** delivers a visual narrative of the data cleaning process, model comparisons, pricing recommendations, and business implications for Airbnb hosts.

---

## 🔎 Key Takeaways

* **Superhost likelihood is strongly correlated** with responsiveness, listing quality, and guest feedback.
* **Data leakage prevention** (removing future or summary-based columns) was essential for honest model performance.
* **Regression and classification pipelines** enabled reusable, scalable analysis for any Airbnb dataset of similar format.
* **Random Forest Regressor** and **XGBoost Classifier** consistently provided the most robust and interpretable results.

---

## 🧑‍💻 Author

**Armand Paul Debray**
MSBAIM Candidate, Purdue University
Air Force Intelligence Officer | Data Analyst | Bilingual (English/French)
🔗 [LinkedIn](https://www.linkedin.com/in/armand-debray-76195b1a5) | 📧 [debray@purdue.edu](mailto:debray@purdue.edu)
