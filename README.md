This project analyzes 9 years (105 months) of airline passenger data to uncover trends, seasonality, and forecast future demand.
Using time series analysis techniques and machine learning models, the project demonstrates an end-to-end pipeline from EDA → stationarity checks → model building → evaluation → forecasting.
The goal is to provide insights that can support airline capacity planning, resource allocation, and demand forecasting.

uses##
Programming: Python
Libraries: pandas, numpy, matplotlib, seaborn, statsmodels, scikit-learn
Modeling: STL Decomposition, ADF/KPSS Tests, SARIMA
Evaluation: RMSE

Project Workflow
*Data Collection & Cleaning
 -Imported 105 months of monthly passenger data.
 -Handled indexing and formatted time series for analysis.
*xploratory Data Analysis (EDA)
  -Visualized trends in passenger growth.
  -Applied STL decomposition to separate trend, seasonality, and residuals.
*Stationarity Testing
  -Conducted ADF & KPSS tests.
  -Applied seasonal differencing (order=12) to achieve stationarity.
*Model Development
  -Used ACF & PACF plots to determine SARIMA parameters.
  -Built a SARIMA(0,1,1)(0,1,1,12) model.
*Model Evaluation
  -Achieved an RMSE ≈ 955, improving over baseline seasonal forecasts.
  -Visualized actual vs. predicted passenger counts.
*Forecasting
  -Forecasted 24 months of future passenger demand.
  -Generated visualizations to highlight future trends for business insights.

Results--
  RMSE: ~955
  Forecast closely tracked actual seasonality and long-term trends.
  Provided 24-month demand forecast for airline planning.

Future Improvements--
  Compare with other models like Prophet or LSTM (Deep Learning).
  Build an interactive dashboard (Tableau / Power BI / Plotly Dash).  
  
