# RETAIL_SLAES_FORECASTING_USING_SARIMA-MODEL


Retail Sales Forecasting using Python and SARIMA. An end-to-end time-series project that analyzes historical monthly sales, identifies trend and seasonality, evaluates potential high-demand periods, forecasts future sales, and compares actual vs predicted values.


Project Overview


This project develops an end-to-end retail sales forecasting solution using historical transaction data. Transaction-level sales are converted into monthly time-series data, followed by trend analysis, seasonal analysis, high-demand-period analysis, SARIMA modeling, model evaluation, and a 12-month future forecast.


Project Objective


Predict future sales based on historical sales.


Prepare transaction data for time-series forecasting.


Identify sales trend and seasonality.


Identify unusually high-sales periods as potential high-demand/promotional periods.


Build and evaluate a SARIMA forecasting model.


Visualize actual vs forecasted sales.


Forecast the next 12 months.



Dataset


The dataset contains approximately 9,800 records and 18 columns. Key fields include Order Date, Sales, Category, Sub-Category, Region, and Segment.


Tools & Technologies


Python, Pandas, NumPy, Matplotlib, Seaborn, Statsmodels, Scikit-learn, Google Colab, GitHub.


Methodology


Data loading and exploratory checks.


Data cleaning and date conversion.


Monthly time-series aggregation.


12-month moving-average trend analysis.


Seasonal decomposition and monthly seasonality analysis.


High-demand/promotional-period analysis.


Augmented Dickey-Fuller stationarity testing.


SARIMA forecasting using SARIMA(1,1,1)(1,1,1,12).


Final-12-month train/test validation.


MAE, RMSE, and MAPE evaluation.


12-month future forecasting.


Key Visualizations


Historical monthly sales


12-month moving-average trend


Seasonal decomposition


Monthly seasonality


Potential high-demand/promotional periods


Actual vs forecasted sales


12-month future forecast with confidence interval


Model Evaluation


The SARIMA model was evaluated on the held-out test period using MAE, RMSE, and MAPE.


Metric	Value


MAE	13,930.02


RMSE	16,394.82


MAPE	27.77%


Interpretation: The model's MAPE of 27.77% indicates that forecasted sales differed from actual sales by approximately 27.77% on average during the test period. MAE and RMSE quantify the average and larger forecast errors in sales units, respectively.


Business Insights


Identify increasing and declining sales periods.


Recognize recurring seasonal demand.


Support inventory and procurement planning.


Investigate unusual high-demand periods.


Support operational and sales planning.


Use confidence intervals to understand forecast uncertainty.


Recommendations


Use forecasts for inventory and procurement planning.


Prepare stock ahead of strong seasonal periods.


Investigate high-sales months to determine whether promotions, holidays, product launches, or other events caused the increase.


Collect explicit promotion, discount, advertising-spend, and holiday variables in future datasets.


Retrain the model as new data becomes available.


Compare SARIMA with Prophet or LSTM when more historical observations are available.


Monitor forecast errors and update the model when performance declines.



Promotional Component Limitation



The dataset does not contain a dedicated promotion, campaign, discount, or advertising-spend field. Therefore, high-sales periods are treated only as potential high-demand/promotional periods and are not confirmed promotions.


Project Structure



Sales-Forecasting/


├── data/train.csv


├── notebooks/Sales_Forecasting.ipynb


├── outputs/sales_forecast_12_months.csv


├── outputs/model_evaluation.csv


├── visualizations/


└── README.md



Conclusion



This project demonstrates a complete retail sales forecasting workflow using Python and SARIMA, combining data preparation, trend and seasonality analysis, high-demand-period analysis, model evaluation, actual-vs-forecast visualization, and future sales forecasting.
