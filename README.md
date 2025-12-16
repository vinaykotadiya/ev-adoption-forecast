# EV / ZEV Forecasting Using Time Series Models

## Research Questions

- How has the adoption of Zero Emission Vehicles (ZEVs) evolved historically compared with petrol, diesel, and hybrid vehicles in the UK?
- What are the key growth trends in ZEV adoption?
- What future trends in ZEV adoption can be inferred from historical data, and how might these trends influence the UK’s transition to sustainable transport?

## Project Overview

This project analyses UK vehicle registration data to understand historical ZEV adoption patterns and to forecast future trends using time-series forecasting models.

## Dataset and Ethics

- Publicly available UK vehicle licensing statistics  
- Quarterly aggregated vehicle registration data  
- Covers multiple fuel types, including petrol, diesel, hybrid, and ZEVs  
- No personal, private, or sensitive information included  
- Data used strictly for academic purposes, posing no ethical or privacy concerns  

## Exploratory Data Analysis and Pre-processing

- Trend analysis shows a strong increase in ZEV registrations over time  
- Quarterly seasonality patterns are visible in the data  
- Time-series decomposition used to examine trend, seasonal, and residual components  
- Data converted into a time-indexed time-series format  
- Stationarity tested using the Augmented Dickey–Fuller (ADF) test  
- Differencing applied where required  
- Data split into training and testing sets, with the last 10 quarters used for testing  

## Models and Model Evaluation

- **ARIMA:** Used to model trend and autocorrelation after differencing  
- **Holt–Winters:** Captures level, trend, and seasonal components  
- **LSTM:** Deep learning model used to learn sequential patterns in the data  

Model parameters were selected manually without hyperparameter optimisation.

- **Evaluation Metric:** Root Mean Squared Error (RMSE)  
- RMSE was derived from Mean Squared Error (MSE) to express prediction error in the original unit (vehicle count)  
- The same evaluation metric was applied to all models to ensure fair comparison  

## Results and Conclusion

- ZEV adoption in the UK shows a clear and accelerating growth trend  
- All implemented models successfully captured the overall trend in the data  
- Forecasting results indicate continued growth in ZEV registrations, supporting the transition towards sustainable transport  

## Author

**Vinay Kotadiya**  
University of Hertfordshire
