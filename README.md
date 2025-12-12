# Walmart Sales Forecasting using the Best ML algorithms

<img width="336" height="686" alt="image" src="https://github.com/user-attachments/assets/2fa071af-a739-4743-b87c-9514c8044dea" />


## 🌐 Live App
You can access the project here: 👉 [Walmart Sales Predictor](https://walmartsalespredictor.streamlit.app/)

Objective

Build an end-to-end Walmart Weekly Sales Forecasting system using regression-based machine learning models. The project covers data cleaning, feature engineering, model training, and model comparison using RMSE as the primary evaluation metric, ultimately selecting the best-performing model for reliable sales prediction.

Project Description

Walmart, one of the largest retail chains in the US, aims to predict weekly sales and demand accurately across 45 stores. Sales are strongly affected by holidays and special events, and Walmart also runs markdown promotions that influence demand—especially around key holidays such as Super Bowl, Labour Day, Thanksgiving, and Christmas.

A major challenge is stock-outs and poor planning caused by inaccurate forecasting. This project builds a robust ML pipeline that incorporates external factors like CPI, unemployment rate, fuel price, and temperature to improve prediction accuracy.

Additionally, holiday weeks are weighted higher than non-holiday weeks, so modeling holiday impact is crucial for strong performance.

Dataset Information

Historical sales data spans 2010-02-05 to 2012-11-01 using the following files:

Key Fields

Store: store ID (1–45)

Date: week of sales

Weekly_Sales: target variable (sales)

IsHoliday: 1 = holiday week, 0 = non-holiday week

Temperature: temperature during the week

Fuel_Price: regional fuel cost

CPI: consumer price index

Unemployment: unemployment rate

Markdown1–5: promotional markdown events (partially missing)

Strategic Planning (Workflow)

Import Libraries (Pandas, NumPy, Scikit-learn, XGBoost, CatBoost, LightGBM)

Load & Merge Datasets (train + features + stores)

Data Exploration (EDA)

sales distribution, holidays effect, store-level trends

Data Preprocessing

handle missing values (esp. markdowns), encoding, scaling where required

Feature Selection / Engineering

date features (year, month, week), store size/type, promotion indicators

Predictive Modeling

train multiple regressors and tune key hyperparameters

Evaluation & Model Selection

compare models using RMSE, pick best model

Conclusion & Insights

summarize best model + business takeaways

Model Evaluation Metrics (RMSE)

RMSE scores obtained:

Linear Regression (LR): 21806.1429

XGBoost (XGB): 5230.9802

CatBoost (CB): 5579.4671

LightGBM (LGB): 6812.8976

Random Forest Regressor (RFR): 3636.2488

✅ Models Ranked by Performance (Best → Worst)

RFR: 3636.2488

XGB: 5230.9802

CB: 5579.4671

LGB: 6812.8976

LR: 21806.1429

Key takeaway: Tree-based ensemble models dramatically outperform linear regression due to non-linear sales patterns, store-level variation, and holiday/promotion effects.
