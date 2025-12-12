# Walmart Sales Forecasting using the Best ML algorithms

<img width="336" height="686" alt="image" src="https://github.com/user-attachments/assets/2fa071af-a739-4743-b87c-9514c8044dea" />


## 🌐 Live App
You can access the project here: 👉 [Walmart Sales Predictor](https://walmartsalespredictor.streamlit.app/](https://walmart-weekly-sales-prediction.streamlit.app/)

# 🏬 Walmart Weekly Sales Forecasting using Machine Learning

## 📌 Objective
Build an **end-to-end Walmart Weekly Sales Forecasting system** using **regression-based machine learning models**.  
The project covers **data cleaning, feature engineering, model training, evaluation, and comparison** using **RMSE** as the primary metric, ultimately selecting the **best-performing model** for reliable sales prediction.

---

## 📖 Project Description
Walmart, one of the largest retail chains in the US, aims to **predict weekly sales and demand accurately** across **45 stores**.  
Sales are heavily influenced by **holidays, promotional markdowns, and economic factors** such as **CPI, fuel prices, temperature, and unemployment rate**.

Inaccurate forecasting leads to **stock-outs and inefficient inventory planning**.  
This project addresses these challenges by building a **robust machine learning pipeline** that captures:
- Holiday and seasonal effects  
- Promotional markdown impacts  
- Store-level variations  
- Macroeconomic indicators  

Special focus is given to major holidays:
- **Super Bowl**
- **Labour Day**
- **Thanksgiving**
- **Christmas**

---

## 📊 Dataset Information
Historical sales data from **2010-02-05 to 2012-11-01**.

### Key Fields
- **Store**: Store ID (1–45)  
- **Dept**: Department number  
- **Date**: Week of sales  
- **Weekly_Sales**: Target variable  
- **IsHoliday**: 1 = Holiday week, 0 = Non-holiday week  
- **Temperature**: Weekly average temperature  
- **Fuel_Price**: Regional fuel cost  
- **CPI**: Consumer Price Index  
- **Unemployment**: Unemployment rate  
- **MarkDown1–5**: Promotional markdown events (partially missing)  
- **Type**: Store category (A/B/C)  
- **Size**: Store size  

---

## 🔄 Project Workflow
1. **Import Libraries**  
   - Pandas, NumPy, Scikit-learn  
   - XGBoost, CatBoost, LightGBM  

2. **Load & Merge Datasets**  
   - Combine `train`, `features`, and `stores`  

3. **Exploratory Data Analysis (EDA)**  
   - Sales distribution  
   - Holiday vs non-holiday impact  
   - Store-level trends  

4. **Data Preprocessing**  
   - Handle missing values (Markdowns)  
   - Encode categorical features  
   - Feature scaling where required  

5. **Feature Engineering**  
   - Date features (Year, Month, Week)  
   - Promotion indicators  
   - Store size and type  

6. **Predictive Modeling**  
   - Linear Regression  
   - Random Forest Regressor  
   - XGBoost  
   - CatBoost  
   - LightGBM  

7. **Model Evaluation & Selection**  
   - Evaluate using **RMSE**  
   - Compare model performance  
   - Select best-performing model  

---

## 📈 Model Evaluation Metrics (RMSE)

| Model | RMSE |
|-----|------|
| **Random Forest Regressor** | **3636.2488** |
| XGBoost | 5230.9802 |
| CatBoost | 5579.4671 |
| LightGBM | 6812.8976 |
| Linear Regression | 21806.1429 |

### 🏆 Models Ranked by Performance
1. **Random Forest Regressor**
2. XGBoost
3. CatBoost
4. LightGBM
5. Linear Regression

**Key Insight:**  
Tree-based ensemble models significantly outperform linear regression due to **non-linear sales patterns, store-level variation, and holiday/promotion effects**.

---

## 📌 Key Insights
- Weekly sales show **high variance and right-skewness**
- Store size and store type strongly influence demand
- Holiday and promotion weeks create sharp sales spikes
- Economic indicators help capture long-term trends
- Ensemble models provide better generalization

---

## ✅ Conclusion
- Built a complete **machine learning pipeline** for Walmart weekly sales forecasting  
- Demonstrated the superiority of **ensemble regression models**  
- **Random Forest Regressor** achieved the best performance with the **lowest RMSE**  
- The system supports **better inventory planning and demand forecasting**

---

## 🧠 One-Line Project Pitch
> *An end-to-end machine learning system that forecasts Walmart weekly sales by leveraging store data, promotions, holidays, and economic indicators using ensemble regression models.*

---

## 📁 Repository Structure
