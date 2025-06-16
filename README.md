# 🌊 Water Pollution Classification in China Using Machine Learning

This project aims to predict and classify the level of **water pollution in China** using supervised machine learning models, **PCA for dimensionality reduction**, and **SHAP for interpretability**.

---

## 📌 Project Goals

- Predict water quality level using physicochemical indicators.
- Reduce class complexity through **binary classification**.
- Understand model decision-making via **SHAP explanations**.
- Identify top contributing features to pollution levels.

---

## 📁 Dataset Overview

The dataset includes several water quality measurements, including:
- `turbidity_ntu`
- `conductivity_us_cm`
- `bod_mg_l`, `cod_mg_l`
- `pH`, `total_nitrogen_mg_l`, `total_phosphorus_mg_l`
- `heavy_metals_cd_ug_l`, `nitrate_mg_l`, `ammonia_n_mg_l`
- And more...

---

## 🧠 Models Used

- Logistic Regression (with and without SMOTE)
- Random Forest
- XGBoost
- Decision Tree
- K-Nearest Neighbors
- Support Vector Classifier

---

## 🧪 Dimensionality Reduction

We applied **Principal Component Analysis (PCA)** and retained the **top 12 components** to reduce noise and improve generalization.

---

## 🧩 Binary Classification Strategy

Due to low accuracy in multiclass classification (~20%), we simplified the target:

- Class 0: _Very Poor, Poor, Moderate_
- Class 1: _Good, Excellent_

This improved model accuracy and interpretability.

---

## 📈 Results Summary

| Model         | Test Accuracy | F1 Macro | F1 Weighted |
|---------------|---------------|----------|--------------|
| Logistic Regression | 0.588 | 0.370 | 0.437 |
| Decision Tree        | 0.588 | 0.408 | 0.467 |
| Support Vector Classifier | 0.580 | 0.404 | 0.462 |
| **Random Forest**        | 0.572 | 0.470 | 0.512 |
| **K-Nearest Neighbors** | 0.568 | **0.522** | **0.549** |
| XGBoost                | 0.540 | 0.486 | 0.516 |

---

## 🔍 SHAP Insights

Using SHAP, we identified the top features contributing to model predictions:

1. `turbidity_ntu`
2. `conductivity_us_cm`
3. `bod_mg_l`
4. `total_phosphorus_mg_l`
5. `pH`
6. `heavy_metals_cd_ug_l`
7. `cod_mg_l`
8. `total_nitrogen_mg_l`
9. `ammonia_n_mg_l`
10. `nitrate_mg_l`

These indicators align with environmental science research, giving us confidence in model transparency.

---

## 🛠️ Technologies Used

- Python
- Pandas, NumPy
- Scikit-learn
- XGBoost
- SHAP
- Matplotlib / Seaborn

---

## 📎 Conclusion

This project demonstrates how machine learning and explainable AI (XAI) can help **classify environmental conditions** and support sustainable decision-making. It also highlights the importance of feature selection, dimensionality reduction, and class simplification in improving model performance.

---

## 📬 Contact

Feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/marthapatriciaortiz/) or explore my other projects!

