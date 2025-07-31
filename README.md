# Global Temperature Change Forecasting
This report seeks to forecast Earth's global temperature changes using Box-Jenkins methodology. NASA's Global Land-Ocean Temperature Index is employed, which contains yearly changes in Earth's global surface temperature compared to the long-term average temperature from 1951-1980.

An ARIMA (autoregressive integrated moving average) model was employed after differencing to remove trend and make sure the time series was stationary. Sample ACF (autocorrelation function) and PACF (partial autocorrelation function) values were used to hypothesize AR (autoregressive) and MA (moving average) model parameters which were compared and selected based on AICc (Akaike Information Criterion corrected for bias) values. Three potential models were chosen with the lowest AICc values and were checked for:
* Stationarity
* Invertibility
* Passing diagnostics

The final model was chosen based upon the principle of parsimony after all three model candidates passed all checks. This ARIMA(0, 1, 2) model was ultimately used to forecast yearly global temperature changes 10-steps ahead. 
