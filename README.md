# 🛒 Walmart Sales Forecasting

## 📌 Project Overview
This project focuses on forecasting weekly sales across different Walmart stores and departments. Accurate sales forecasting helps Walmart optimize **inventory management**, **supply chain decisions**, and **promotional planning**.

The dataset contains historical sales data, holiday information, and economic indicators such as **CPI**, **Unemployment Rate**, and **Fuel Price**.

---

## 📂 Dataset
- **Store**: Store ID  
- **Dept**: Department ID  
- **Date**: Week of sales  
- **Weekly_Sales**: Sales for the given store/department/date (Target)  
- **Holiday_Flag**: Indicates whether the week includes a holiday  
- **Temperature**: Average temperature of the region  
- **Fuel_Price**: Cost of fuel in the region  
- **CPI**: Consumer Price Index  
- **Unemployment**: Unemployment rate of the region  

---

## 🔧 Approach
1. **Data Preprocessing**
   - Handled missing values
   - Converted dates to time features (Year, Month, Week)
   - Created lag/rolling features for sales trends

2. **Exploratory Data Analysis (EDA)**
   - Analyzed sales trends across stores & departments
   - Studied the impact of holidays
   - Correlation analysis with economic factors

3. **Feature Engineering**
   - Added holiday/weekend indicators
   - Created lag and moving average features
   - Encoded categorical variables

4. **Modeling**
   - ARIMA (time-series forecasting model)
   - Evaluated using **Mean Squared Error (MSE) / Root Mean Squared Error (RMSE)**

---

## 📊 Results
- The **ARIMA model** provided reasonable sales forecasts.
- Sales showed strong **seasonality** with spikes during **holiday weeks**.
- Economic indicators (CPI, Unemployment) were weaker predictors compared to **seasonality and holiday effects**.

---

## 🚀 Future Improvements
- Experiment with machine learning models (XGBoost, LightGBM, Random Forest).
- Incorporate deep learning models (LSTMs, Transformers).
- Use additional external data (weather, promotions, events).
- Deploy the model as an **API for real-time forecasting**.

---

## 📌 Tech Stack
- **Python**
- Pandas, NumPy
- Matplotlib, Seaborn
- Statsmodels (ARIMA)
- Scikit-learn (evaluation metrics)

---

## 📜 License
This project is open-source and available under the MIT License.
