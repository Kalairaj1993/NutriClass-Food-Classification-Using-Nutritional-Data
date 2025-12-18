---

# 🥗 NutriClass – Food Classification Using Nutritional Data

An **end-to-end machine learning project** that builds, evaluates, and compares multiple traditional ML models to classify food items into predefined categories using **tabular nutritional data** such as calories, protein, carbohydrates, fat, sugar, fiber, sodium, and cholesterol.

The project covers **data preprocessing, feature engineering, model benchmarking, evaluation metrics, visualizations**, and **model artifact generation** for deployment readiness.

---

## 📌 Project Overview

With the growing focus on healthy eating and nutrition awareness, accurately categorizing food based on nutritional composition is essential. **NutriClass** aims to automatically classify food items into meaningful food categories using nutritional attributes.

This project demonstrates how **traditional machine learning algorithms** can effectively solve multi-class classification problems using structured nutritional data.

---

## 🚀 Problem Statement

Design and develop a machine learning system that can accurately classify food items into predefined food categories (e.g., beverages, fruits, vegetables, grains, proteins, desserts) using their nutritional values.

The project involves:

* Understanding nutritional data
* Cleaning and preprocessing
* Feature scaling and dimensionality analysis
* Training multiple ML models
* Comparing performance using robust evaluation metrics
* Extracting insights from model behavior

---

## 🎯 Business Use Cases

### 1️⃣ Smart Dietary Applications

Recommend foods based on balanced nutritional profiles.

### 2️⃣ Health Monitoring Tools

Assist dieticians and nutritionists in categorizing food efficiently.

### 3️⃣ Food Logging Systems

Automatically classify foods entered by users in health-tracking apps.

### 4️⃣ Educational Platforms

Demonstrate relationships between nutrients and food categories.

### 5️⃣ Grocery & Meal Planning Apps

Suggest healthier alternatives within the same food category.

---

## 🧭 Project Workflow

### 1️⃣ Data Understanding & Exploratory Data Analysis (EDA)

* Loaded nutritional dataset (CSV-based)
* Examined:

  * Class distribution
  * Summary statistics
  * Feature correlations
* Visualizations:

  * Class count plots
  * Pairplots (sample-based)
  * Correlation heatmaps

---

### 2️⃣ Data Preprocessing

* Removed duplicate records
* Handled missing values using **median imputation**
* Treated outliers using **IQR-based capping**
* Standardized numerical features using **StandardScaler**
* Encoded target labels using **Label Encoding**

---

### 3️⃣ Feature Engineering

* Numerical feature selection
* Optional dimensionality analysis using:

  * **Principal Component Analysis (PCA)** (explained variance inspection)
* Prepared clean feature matrix for modeling

---

### 4️⃣ Model Training & Selection

The following machine learning models were trained and evaluated:

| Model                  | Description                   |
| ---------------------- | ----------------------------- |
| Logistic Regression    | Strong linear baseline        |
| Decision Tree          | Interpretable, non-linear     |
| Random Forest          | Ensemble, reduced overfitting |
| K-Nearest Neighbors    | Distance-based                |
| Support Vector Machine | High-dimensional classifier   |
| Gradient Boosting      | Strong ensemble learner       |
| XGBoost (Optional)     | Boosting-based model          |

* Used **train-test split (80/20)**
* Applied **5-fold cross-validation**
* Ensured reproducibility with `random_state`

---

## 📊 Model Evaluation Metrics

Each model was evaluated using:

* Accuracy
* Precision (weighted)
* Recall (weighted)
* F1-score (weighted)
* Confusion Matrix

---

## 📈 Consolidated Model Performance

| Model                 | CV Accuracy | Test Accuracy | Precision | Recall | F1-score |
| --------------------- | ----------: | ------------: | --------: | -----: | -------: |
| **Decision Tree**     |      0.9996 |    **1.0000** |    1.0000 | 1.0000 |   1.0000 |
| **Gradient Boosting** |      0.9997 |    **1.0000** |    1.0000 | 1.0000 |   1.0000 |
| Random Forest         |      0.9994 |        0.9998 |    0.9998 | 0.9998 |   0.9998 |
| Logistic Regression   |      0.9851 |        0.9861 |    0.9859 | 0.9861 |   0.9860 |
| SVM                   |      0.9839 |        0.9849 |    0.9847 | 0.9849 |   0.9847 |
| KNN                   |      0.9519 |        0.9493 |    0.9492 | 0.9493 |   0.9490 |

---

## 🏆 Best Performing Models

* **Decision Tree & Gradient Boosting**
* Achieved **100% test accuracy and F1-score**
* Demonstrated excellent class separation

---

## 📊 Visualizations Included

✔ Class distribution plots

✔ Correlation heatmaps

✔ PCA explained variance plot

✔ Model accuracy comparison bar chart

✔ Confusion matrix heatmaps

✔ Feature importance plots (tree-based models)

---

## 🔍 Feature Importance Insights

Tree-based models highlighted the following as dominant predictors:

* Calories
* Sugar
* Fat
* Protein
* Carbohydrates

These features strongly influence food category separation.

---

## 💾 Model Artifacts

Saved for deployment and reuse:

* Trained best model
* Feature scaler
* Label encoder

Stored in the `artifacts/` directory using **Joblib**.

---

## 🧪 Project Structure

```
NutriClass-Food-Classification-Using-Nutritional-Data/
│
├── data/                # CSV dataset
├── notebooks/           # Jupyter notebooks
├── README.md
└── requirements.txt
```

---

## 🔮 Future Enhancements

* Feature ratios (protein/calories, fat/calories)
* Class-weighted training for real-world imbalance
* Stacking & ensemble blending
* Model tracking using MLflow
* Deployment using FastAPI or Flask
* Replace synthetic data with real-world labeled datasets

---

## 🤝 Contributions

Contributions, issues, and feature requests are welcome.

---

## 📧 Contact

**Kalairaj**
📊 Data Analyst & Developer
📧 Email: **[rajfreelancer1993@gmail.com](mailto:rajfreelancer1993@gmail.com)**

---
