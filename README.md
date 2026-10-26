# Global-Container-Freight-Rate-Forecasting

1. Introduction & Motivation
This project focuses on the analysis and forecasting of the Baltic Dry Index (BDI), a leading economic indicator issued daily by the London-based Baltic Exchange. The BDI tracks the cost of shipping major raw materials (iron ore, coal, grain) across more than 20 global shipping routes.

Unlike standard stock market indices, the BDI is a pure measure of supply and demand for shipping capacity. It is often cited by economists as a precursor to global economic activity because it is devoid of speculative bubbles — materials are only shipped when there is actual industrial demand.

2. Project Objectives
The primary goal is to develop a robust statistical pipeline to forecast the BDI Price variable. Specifically, this project aims to:

Analyse historical volatility and seasonality of BDI over 2016–2026.
Formally test for stationarity using both ADF and KPSS tests.
Select optimal ARIMA orders through systematic grid search (AIC/BIC).
Model the series using ARIMA and Holt-Winters Exponential Smoothing.
Validate model quality via residual diagnostics (Ljung-Box, Q-Q plot, ACF of residuals).
Forecast BDI for Q1/Q2 2026 and evaluate accuracy with 95% confidence intervals.
Assess business impact for shipping operators.
3. Dataset Description
Dataset: Baltic Dry Index Historical Data from investing.com.

Span: Daily data from April 2016 – April 2026 (2,512 trading days).
Key Variable: Price (BDI index value).
Frequency: Daily (business days); resampled to weekly for modelling.
