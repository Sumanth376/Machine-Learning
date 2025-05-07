# 🍽️ Forecasting Monthly Restaurant Sales

## 📌 Problem Statement

Accurately forecasting restaurant sales is critical for operational efficiency, including inventory management, staffing, and promotional planning. This project addresses the challenge by developing a **time series forecasting model** that predicts monthly restaurant sales using historical data. With better predictions, the restaurant can streamline resources, reduce waste, and increase profitability.

---

## 🎯 Objectives

- Analyze historical sales data to identify trends and seasonality  
- Preprocess and visualize monthly sales data  
- Apply various time series forecasting models (e.g., ARIMA, Prophet, XGBoost)  
- Evaluate models using relevant forecasting metrics  
- Forecast sales for the next 6 months  
- Provide visual insights into trends, seasonality, and forecast accuracy  

---

## 🧩 Dataset Overview

The dataset consists of 156 monthly records from **January 2010 to December 2022** with the following features:

- `Date` – Month-end date of the sales record  
- `Sales` – Total monthly sales in USD  

**Summary Statistics**:
- Time Range: *Jan 2010 – Dec 2022*  
- Mean Sales: *$2,671*  
- Max Sales: *$6,241*  
- Min Sales: *$10.50*  

---

## 🧪 Data Preprocessing & Feature Engineering

- Converted `Date` column to datetime format and set it as time series index  
- Handled missing values (if any) and verified consistency of time intervals  
- Decomposed time series into trend, seasonal, and residual components  
- Created lag features and rolling averages (where applicable) for modeling  

---

## 🤖 Model Building

### Models used:

- **ARIMA (AutoRegressive Integrated Moving Average)**  
- **Facebook Prophet**  
- **XGBoost Regressor**  

### Model evaluation metrics:

- **Mean Absolute Error (MAE)**  
- **Root Mean Squared Error (RMSE)**  
- **Mean Absolute Percentage Error (MAPE)**  

> Facebook Prophet and ARIMA models demonstrated strong forecasting performance, with low error metrics and interpretable seasonality.

---

## 📊 Visualizations

- Time series plot of monthly sales  
- Seasonal decomposition (trend, seasonality, residuals)  
- Forecast vs Actual plots  
- Error distribution and evaluation metric comparison  
- Prophet model's trend and seasonal component charts  

---

## 🔍 Key Insights

- Clear seasonal trends were observed, with sales typically peaking during certain months (e.g., holidays)  
- Long-term upward sales trend from 2010–2019, slight instability during pandemic years  
- Prophet model effectively captured holidays and trends  
- Time series models are sensitive to sudden external disruptions (e.g., COVID-19 effects)  

---

## 🛠️ Technologies Used

- Python, Pandas, NumPy, Seaborn, Matplotlib  
- Statsmodels (for ARIMA), Facebook Prophet, XGBoost  
- Scikit-learn (for preprocessing and metrics)  
- Jupyter Notebook  
- Git & GitHub for version control  

---

## 🚀 Future Improvements

- Incorporate external factors like holidays, events, weather, and promotions for better accuracy  
- Test SARIMA or LSTM models for long-term sequence learning  
- Build a dashboard (e.g., Streamlit) for interactive forecasting  
- Automate data pipeline for real-time monthly updates  
