# 🚖 Taxi Trip Price Prediction & Hypothesis Testing

![taxi_1](https://github.com/user-attachments/assets/2fb7ac69-45e5-4e52-97ab-7c3a169bff0a)

This project aims to analyze and model taxi trip data to **predict trip prices** using machine learning and statistical analysis. It includes **data preprocessing, exploratory data analysis (EDA), hypothesis testing**, and the implementation of **linear and polynomial regression models**.

---

## 📂 Dataset Source

The dataset used for this project is publicly available on Kaggle:  
👉 [Kaggle Dataset – Taxi Price Prediction](https://www.kaggle.com/datasets/denkuznetz/taxi-price-prediction)

---

## 📌 Project Overview

The main goals of this project are:

* Understand relationships between taxi trip variables.
* Use **OLS regression and hypothesis testing** to identify statistically significant predictors.
* Build **predictive models** for estimating trip prices.
* Evaluate model performance and **persist trained models** for future use.

---

## 🚀 Getting Started

### Clone the repository
```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```
### OR Direct Download Pkl models for testing

[taxi_linear_model](https://github.com/Monike123/Taxi_Fare_Analysis/blob/main/taxi_linear_model.pkl)

[taxi_ploy_linear_model](https://github.com/Monike123/Taxi_Fare_Analysis/blob/main/taxi_ploy_linear_model.pkl)

---

## 🧱 Project Workflow

### 1. 📥 Data Loading & Preprocessing

* Load the taxi trip pricing dataset.
* Handle missing values and ensure data quality.
* Prepare the data for analysis and modeling.

### 2. 📊 Exploratory Data Analysis (EDA)

* Visualize distributions using histograms and pairplots.
* Use scatter plots to explore feature relationships:

  * Base Fare vs. Per Km Rate
  * Base Fare vs. Per Minute Rate
  * Trip Distance vs. Trip Price

### 3. 🧪 Hypothesis Testing

* Conduct statistical tests using **Ordinary Least Squares (OLS)** regression.
* Evaluate:

  * **R-squared**
  * **F-test p-value**
  * Significant predictors (p < 0.05)
* Decide whether to **reject or accept null hypotheses** (H₀) for each target feature.

### 4. 🤖 Machine Learning Models

#### 🔹 Linear Regression

* Trained using features such as distance, duration, and fare components.
* Evaluated on test data.

#### 🔹 Polynomial Regression (Degree = 6)

* Captures non-linear feature relationships.
* Trained and evaluated similarly to linear regression.

### 5. 📈 Model Evaluation

* Metrics:

  * **Mean Squared Error (MSE)**
  * **R-squared (R²)**
* Compare performance between linear and polynomial models.

### 6. 💾 Model Persistence

* Save trained models using **Pickle**.
* Demonstrates how models can be reused for **new predictions** without retraining.

---

## 🛠️ Tools & Libraries

* Python 3.x
* `pandas`, `numpy`
* `matplotlib`, `seaborn`
* `statsmodels`
* `sklearn`
* `pickle`

---

## 📎 Example Hypothesis Test

**Test:**

> Is there a significant relationship between `Trip_Price` and features like `Trip_Distance_km`, `Base_Fare`, etc.?

**Null Hypothesis (H₀):** No significant relationship  
**Alternative Hypothesis (H₁):** At least one predictor has a significant effect

✅ Output includes:

* R² value
* F-test p-value
* Significant predictors
* Decision to reject or accept H₀

---

## 📂 Project Structure

```bash
├── taxi_analysis.ipynb         # Main notebook with all analysis
├── models/
│   ├── linear_model.pkl        # Saved linear regression model
│   └── poly_model.pkl          # Saved polynomial regression model
├── data/
│   └── taxi_trip_pricing.csv   # Dataset used in this project
```

## ✅ Future Work
* Try other models (e.g., Random Forest, XGBoost).
* Add interactive dashboard with Streamlit or Flask.
* Enhance feature engineering (e.g., time of day, weekday/weekend).
![taxi2](https://github.com/user-attachments/assets/738be1d6-3637-47d6-be19-886e1696ecda)

