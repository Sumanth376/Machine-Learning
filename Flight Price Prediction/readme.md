# ✈️ Flight Price Prediction

## 📌 Problem Statement

Flight pricing is dynamic and influenced by numerous factors such as departure time, arrival time, number of stops, airline, source, destination, and duration. For travelers and travel agencies alike, it is often challenging to predict the cost of a flight ticket at a given time due to these fluctuating conditions.

This project aims to solve the problem by building a **machine learning regression model** that can accurately predict flight prices using historical data and engineered features. The insights generated can help users book flights more economically and help travel agencies optimize their pricing strategies.

---

## 🎯 Objectives

- Analyze and understand the factors affecting flight ticket prices  
- Preprocess and clean flight data for model consumption  
- Perform feature engineering (e.g., extracting date-time components, calculating duration)  
- Train and evaluate multiple regression models for price prediction  
- Identify the most important features influencing price  
- Deploy or visualize the model for practical use  

---

## 🧩 Dataset Overview

The dataset includes the following features:

- `Date_of_Journey` – Journey date of the passenger  
- `Airline` – The airline the passenger has chosen  
- `Source` – Source city of the flight  
- `Destination` – Destination city of the flight  
- `Route` – Path of the flight  
- `Dep_Time` / `Arrival_Time` – Departure and arrival times  
- `Duration` – Total duration of the flight  
- `Total_Stops` – Number of stops  
- `Price` – Target variable (flight fare)  

---

## 🧪 Data Preprocessing & Feature Engineering

- Converted `Date_of_Journey`, `Dep_Time`, `Arrival_Time` to datetime objects and extracted day, month, hour, minute  
- Calculated duration in minutes  
- Cleaned missing values and inconsistencies  
- Encoded categorical variables using Label Encoding and One-Hot Encoding  
- Dropped irrelevant/redundant columns like `Route`, `Additional_Info`  

---

## 🤖 Model Building

### Models used:

- Linear Regression  
- Decision Tree Regressor  
- Random Forest Regressor  
- XGBoost Regressor  

### Model evaluation metrics:

- **R² Score**  
- **Root Mean Squared Error (RMSE)**  
- **Mean Absolute Error (MAE)**  

> Random Forest and XGBoost showed the best performance with high R² and low RMSE.

---

## 📊 Visualizations

- Correlation heatmap for feature relationships  
- Feature importance bar chart for top predictors  
- Distribution plots of target and input variables  
- Error distribution plot (Predicted vs Actual)  

---

## 🔍 Key Insights

- Flight duration, number of stops, and airline have a significant impact on ticket price  
- Non-stop flights are generally costlier  
- Evening and night flights often differ in pricing compared to morning flights  
- Some airlines consistently have higher pricing across routes  

---

## 🛠️ Technologies Used

- Python, Pandas, NumPy, Seaborn, Matplotlib  
- Scikit-learn, XGBoost  
- Jupyter Notebook  
- Git & GitHub for version control  

---

## 🚀 Future Improvements

- Include real-time or larger dataset for improved accuracy  
- Integrate web scraping to fetch latest flight data  
- Build a Streamlit/Flask app for user-friendly flight price predictions  
- Use hyperparameter tuning techniques like GridSearchCV  
