# AdClick Predictor: Machine Learning Classification Pipeline

An end-to-end Machine Learning pipeline designed to predict user engagement on digital advertisements based on demographic and behavioral metrics. Built using Python, Scikit-Learn, Pandas, and Seaborn.

---

## 📌 Project Overview

Digital marketing campaigns rely heavily on targeted ad delivery. This project implements a Logistic Regression classification pipeline that analyzes user behavior patterns—such as daily time spent on site, internet usage, age, and area income—to predict whether a user is likely to click on an advertisement (`1`) or not (`0`).

---

## Key Features

* **Modular Data Pipeline:** Uses Scikit-Learn's `ColumnTransformer` and `Pipeline` for leakage-free feature scaling and pre-processing.
* **Standardized Scaling:** Applies `StandardScaler` to continuous numerical features while keeping binary features clean with `passthrough`.
* **Exploratory Visualizations:** Pairplot distributions generated via Seaborn to inspect cross-feature interactions and class separability.
* **Model Evaluation:** Detailed performance benchmarking using precision, recall, and F1-score via `classification_report`.

---

## 📁 Dataset Features

| Feature Name | Description | Preprocessing |
| :--- | :--- | :--- |
| `Daily Time Spent on Site` | Daily time spent on the platform (minutes) | Standardized |
| `Age` | User age in years | Standardized |
| `Area Income` | Average income of the user's geographic region | Standardized |
| `Daily Internet Usage` | Daily internet consumption (minutes) | Standardized |
| `Male` | Gender indicator (`1` = Male, `0` = Female) | Passthrough |
| **`Clicked on Ad`** | **Target Variable** (`1` = Clicked, `0` = Did Not Click) | Label |

---

## Tech Stack

* **Language:** Python 3.10+
* **Data Processing:** `Pandas`, `NumPy`
* **Machine Learning:** `Scikit-Learn` (`LogisticRegression`, `Pipeline`, `ColumnTransformer`)
* **Data Visualization:** `Seaborn`, `Matplotlib`

---
