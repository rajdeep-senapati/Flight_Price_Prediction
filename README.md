# ✈️ Flight Fare Prediction – Machine Learning Project

## 📌 Project Overview

This project aims to predict flight ticket prices using supervised machine learning techniques. By analyzing various flight features like airline, source, destination, duration, and number of stops, the model predicts the most likely price a customer would pay, helping businesses optimize pricing strategies.

---

## 📁 Project Structure

- `FlightPrediction.ipynb` – Jupyter Notebook containing the full analysis and modeling workflow
- `Data_Train.xlsx` – Dataset containing historical flight information (assumed)
- Model performance metrics and visualizations included in the notebook

---

## 🛠️ Tools & Libraries Used

- **Python** (Jupyter Notebook)
- **Libraries**:
  - `pandas`, `numpy` – for data loading and preprocessing
  - `matplotlib`, `seaborn` – for visual exploration
  - `sklearn` – for machine learning algorithms and evaluation
  - `xgboost` – for advanced boosting-based regression

---

## 🔍 Key Steps Performed

### 1. Data Cleaning & Preprocessing
- Converted date/time features to numerical values (e.g., journey date, departure/arrival time)
- Extracted total duration in minutes
- Handled categorical variables using **OneHotEncoding** and **LabelEncoding**
- Removed unnecessary or redundant columns (e.g., route with missing values)

### 2. Exploratory Data Analysis (EDA)
- Explored price distributions across airlines, sources, destinations, and stops
- Checked correlations between features and target variable (`Price`)
- Visualized top airlines and their impact on fare prices

### 3. Feature Engineering
- Extracted day, month, hour from date/time fields
- Derived features such as `Total_Stops`, `Journey_day`, `Journey_month`, `Duration_mins`

### 4. Model Building
- Trained multiple regression models:
  - **Linear Regression**
  - **Decision Tree Regressor**
  - **Random Forest Regressor**
  - **XGBoost Regressor**
- Used **GridSearchCV** for hyperparameter tuning

### 5. Model Evaluation
- Compared models using:
  - R² Score
  - MAE (Mean Absolute Error)
  - RMSE (Root Mean Squared Error)
- **XGBoost** yielded the best performance

---

## 📈 Key Insights

- Airlines and total duration have a significant effect on price
- Weekend and early-morning flights often cost more
- XGBoost provides the most accurate predictions due to its ability to handle complex patterns

---

## ✅ Outcome

- Final model predicts flight prices with high accuracy
- Useful for travel agencies, booking platforms, and customers to estimate costs
- Can be extended into a full-fledged fare recommendation engine

---

## 📌 Author

**Rajdeep Senapati**  
B.Tech in CSE (Data Science)  
[LinkedIn](https://www.linkedin.com/in/rajdeep-senapati) • [GitHub](https://github.com/rajdeep-senapati)

---

## 📂 License

This project is intended for educational and non-commercial use only.
