# Walmart-Sales-Forecasting-Using-SARIMAX-with-Economic-Indicators

https://colab.research.google.com/drive/1jWjxn0pWrVGjZnD-rkbY13_Zyz5ZoL1-#scrollTo=1e2QSho1uDbP

## Project Overview

This project focuses on forecasting Walmart weekly sales using the SARIMAX (Seasonal AutoRegressive Integrated Moving Average with Exogenous Variables) model. The model incorporates historical sales data along with external economic indicators such as Fuel Price, Consumer Price Index (CPI), Unemployment Rate, Temperature, and Holiday effects to improve forecasting performance.

---

## Dataset Information

* Dataset: Walmart Sales Dataset
* Store Selected: Store 1
* Target Variable: Weekly_Sales
* Time Period: 2022 – 2024
* Total Records: 143 Weekly Observations

### Features Used

| Feature      | Description                              |
| ------------ | ---------------------------------------- |
| Weekly_Sales | Weekly store sales (Target Variable)     |
| Holiday_Flag | Indicates holiday week (0 = No, 1 = Yes) |
| Temperature  | Weekly temperature                       |
| Fuel_Price   | Fuel price during the week               |
| CPI          | Consumer Price Index                     |
| Unemployment | Unemployment rate                        |

---

## Project Workflow

Walmart Dataset
↓
Data Preprocessing
↓
Exploratory Data Analysis
↓
Target Variable Selection (Weekly Sales)
↓
Exogenous Variable Selection
↓
Train-Test Split (80:20)
↓
Auto ARIMA Model Selection
↓
SARIMAX Model Development
↓
Forecasting
↓
Model Evaluation
↓
Future Sales Prediction

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Statsmodels
* pmdarima
* Scikit-learn
* Google Colab

---

## Model Development

### Target Variable

* Weekly_Sales

### Exogenous Variables

* Holiday_Flag
* Temperature
* Fuel_Price
* CPI
* Unemployment

### Model Used

SARIMAX (Seasonal AutoRegressive Integrated Moving Average with Exogenous Variables)

Best Model:

SARIMAX(2,0,2)(1,0,0,52)

---

## Key Findings

| Variable     | Impact on Sales |
| ------------ | --------------- |
| Holiday_Flag | Positive Impact |
| Temperature  | Negative Impact |
| Fuel_Price   | Positive Impact |
| CPI          | Positive Impact |
| Unemployment | Negative Impact |

### Statistical Significance

All economic indicators were found to be statistically significant with p-values below 0.05.

---

## Forecast Results

The SARIMAX model forecasts that Walmart Store 1 weekly sales will remain between approximately:

* $1.49 Million
* $1.60 Million

during the next 12 weeks.

Highest Forecasted Sales:

* Week Ending: 29-Dec-2024
* Forecast Sales: Approximately $1.60 Million

---

## Future Forecast Visualization

The forecast trend indicates stable weekly sales with moderate fluctuations influenced by economic conditions and holiday effects.

---

## Business Insights

* Holiday periods significantly increase weekly sales.
* CPI and Fuel Price have a strong influence on sales performance.
* Higher unemployment rates negatively affect consumer spending.
* Temperature variations impact weekly purchasing behavior.

---

## Conclusion

This project demonstrates the effectiveness of SARIMAX for retail sales forecasting by incorporating external economic indicators. 
The model successfully captures relationships between sales and macroeconomic factors, providing valuable insights for demand planning, inventory management,
and business decision-making.

---

## Prepared by

Sugumar Ranganathan
