# 🌍 Air Quality Index (AQI) Prediction using Machine Learning

## 📌 Overview

This project focuses on predicting the **Air Quality Index (AQI)** using machine learning techniques based on major air pollutants such as **CO, NO₂, Ozone, and PM2.5**, along with **geographical features (latitude & longitude)**.

The goal is to build an accurate predictive model that can help in:

* Monitoring environmental pollution
* Supporting public health decisions
* Enabling data-driven policy planning

---

## 🎯 Problem Statement

Air pollution is a major global concern affecting millions of people. Accurate AQI prediction can:

* Help governments issue early warnings
* Enable citizens to take preventive measures
* Support environmental agencies in decision-making

This project aims to **predict AQI values based on pollutant concentrations** using machine learning models.

---

## 📊 Dataset Description

The dataset contains air quality and geographic data with the following features:

| Feature Name    | Description                         |
| --------------- | ----------------------------------- |
| AQI Value       | Target variable (Air Quality Index) |
| CO AQI Value    | Carbon Monoxide concentration       |
| Ozone AQI Value | Ozone level                         |
| NO2 AQI Value   | Nitrogen Dioxide level              |
| PM2.5 AQI Value | Fine particulate matter             |
| Latitude (lat)  | Geographic coordinate               |
| Longitude (lng) | Geographic coordinate               |

---

## 🔍 Exploratory Data Analysis (EDA)

Performed detailed EDA to understand:

* Data distribution (histograms)
* Feature relationships (pairplots)
* Correlation between variables (heatmap)
* Outliers and skewness

### 📈 Key Insights:

* PM2.5 and NO₂ strongly influence AQI
* Some features show multicollinearity
* Geographic features introduce spatial variation

---

## ⚙️ Data Preprocessing

* Removed missing values
* Standardized column names
* Feature scaling using **StandardScaler**
* Train-test split (80-20)

---

## 🧠 Feature Engineering

Created additional features to improve model performance:

* **Pollution Sum** = CO + NO₂
* **Pollution Ratio** = PM2.5 / Ozone

These features help capture **combined pollutant effects**.

---

## 🤖 Models Used

Multiple models were implemented and compared:

* Linear Regression
* Random Forest Regressor
* Gradient Boosting Regressor

---

## 🔥 Hyperparameter Tuning

Used **RandomizedSearchCV** to optimize the Random Forest model:

* n_estimators
* max_depth
* min_samples_split

This improved model performance significantly.

---

## 📊 Model Evaluation Metrics

Models were evaluated using:

* **MAE (Mean Absolute Error)**
* **RMSE (Root Mean Squared Error)**
* **R² Score**

These metrics help assess prediction accuracy and error distribution.

---

## 📉 Model Comparison

| Model             | MAE | RMSE | R² Score |
| ----------------- | --- | ---- | -------- |
| Linear Regression | ... | ...  | ...      |
| Random Forest     | ... | ...  | ...      |
| Gradient Boosting | ... | ...  | ...      |

*(Fill values from your results)*

---

## 📈 Visualizations

* Feature correlation heatmap
* Distribution plots
* Pairplots
* Actual vs Predicted AQI graph
* Model comparison bar chart

---

## ⚠️ Classification Metrics (Extended Analysis)

To include classification evaluation:

* AQI values were categorized into levels (Good, Moderate, Poor)
* Applied classification model
* Evaluated using:

  * Confusion Matrix
  * ROC-AUC Curve

---

## 💾 Model Saving

Final model was saved using:

```python
import joblib
joblib.dump(model, 'aqi_model.pkl')
```

---

## 🚀 Future Improvements

* Deploy model using **Streamlit / Flask**
* Integrate real-time AQI APIs
* Use advanced models like:

  * XGBoost
  * CatBoost
* Improve feature engineering with weather data

---

## 🛠️ Tech Stack

* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn

---

## 📂 Project Structure

```
AQI-Prediction/
│── data/
│── notebooks/
│── model/
│── README.md
```

---

## 💡 Key Learnings

* Importance of EDA in understanding data
* Feature engineering improves model accuracy
* Model comparison helps choose best algorithm
* Hyperparameter tuning boosts performance

---

## 📌 Conclusion

The project successfully predicts AQI using machine learning models, with **Random Forest performing the best** after tuning.

This solution demonstrates how data-driven techniques can help tackle real-world environmental problems.

---

