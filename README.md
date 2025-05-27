
# 🏙️ Air Quality Index (AQI) Prediction

This project builds a regression model to predict the Air Quality Index (AQI) based on various environmental pollutant levels collected from Indian cities. It also includes visualizations of regional pollution trends across the country.

---

## 📌 Problem Statement

To predict AQI values using features such as PM2.5, PM10, NO2, SO2, CO, and O3 using regression models. The model helps in assessing pollution severity and forecasting future air quality, especially in highly polluted urban areas of India.

---

## 📂 Dataset

- **Source:** [Kaggle – Air Quality Data in India by Rohan Rao](https://www.kaggle.com/datasets/rohanrao/air-quality-data-in-india)
- **Cities Covered:** 29 Indian cities
- **Time Range:** 2015 to 2020
- **Key Features:**  
  - `PM2.5`, `PM10`, `NO2`, `SO2`, `CO`, `O3`  
  - `AQI` (Target Variable)

---

## 🛠️ Technologies Used

- **Programming Language:** Python
- **Libraries:**  
  - Data Processing: `pandas`, `numpy`  
  - Modeling: `scikit-learn`, `xgboost`, `randomforest`  
  - Visualization: `matplotlib`, `seaborn`  

---

## 🧪 Methodology

1. **Data Cleaning:**  
   - Removed missing values from AQI and pollutant features  
   - Applied forward/backward fill for other missing data

2. **Feature Selection:**  
   - Selected relevant pollutants as input features

3. **Preprocessing:**  
   - Scaled features using `StandardScaler`  
   - Train-test split (80:20)

4. **Modeling:**  
   - Trained and evaluated multiple regression models:  
     - Linear Regression  
     - Random Forest Regressor  
     - XGBoost Regressor  

5. **Evaluation Metrics:**  
   - Mean Absolute Error (MAE)  
   - Mean Squared Error (MSE)  
   - R² Score  

---

## 📈 Results

| Model              | MAE   | MSE    | R² Score |
|-------------------|-------|--------|----------|
| Linear Regression | 28.4  | 1250.7 | 0.78     |
| Random Forest     | 23.5  | 1054.6 | 0.87     |
| XGBoost           | 22.1  | 985.3  | 0.89     |

- **XGBoost performed best** among all tested models.
- High accuracy in predicting AQI across most cities.

---

## 📊 Visualizations

- **Correlation Heatmap** of pollutants
- **Feature Importance Plot** from Random Forest
- **Predicted vs Actual AQI** scatter plot
- **Average AQI by City** bar chart

---

## 📍 Key Insights

- **PM2.5** and **PM10** are the most significant predictors of AQI.
- **Delhi, Kanpur, Lucknow** showed consistently poor air quality.
- **Coastal cities** like **Chennai and Mumbai** had better air quality levels.

---

## ✅ How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/AQI-Prediction.git
   cd AQI-Prediction

