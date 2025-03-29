# Super Bowl LIX Handle Projection
## Forecasting U.S. Sports Betting Handle: Super Bowl 59
This project forecasts monthly U.S. sports betting handle and ultimately, estimates the total legal wagers for Super Bowl 59 (February 2025). With the rapid growth of legalized betting across states, the Super Bowl continues to draw record-setting wagers. This project uses time series techniques to quantify and project these trends.

## Project Goals
- Forecast total monthly U.S. sports betting handle
- Estimate Super Bowl 59 betting handle from projected February 2025 values
- Identify and quantify the influence of factors such as seasonality, number of legal states, and number of major sports in season

##  Methods & Models
The project walks through the full modeling pipeline:
1. **Data Wrangling**: Monthly handle, revenue, and tax data from LegalSportsReport, combined with legal state counts and sports calendars
2. **Exploratory Analysis**:
    - Trend and seasonality decomposition using STL
    - Feature engineering for sports-in-season and legalization metrics
3. **Modeling**:
    - TSLM (Time Series Linear Model)
    - ETS (Exponential Smoothing)
    - ARIMA
    - SARIMA (Seasonal ARIMA) — selected as final model
4. **Forecasting**:
    - Monthly handle projected through February 2025
    - Super Bowl handle inferred as a % of February totals based on historical ratios
  
## Key Results
**SARIMA Model**: ARIMA(0,1,0)(0,1,0)[12] chosen for its accuracy and stability

Forecasted Super Bowl 59 Handle: **$2.59 billion**
