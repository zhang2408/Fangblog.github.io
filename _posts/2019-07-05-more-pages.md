---
layout: post
title: Two Methods to Predict Stock Index
author: Chenlu Wang
date: 2019-08-02
---

<!-- more -->

<p style="text-align:justify">
The stock price is a typical time series column data (referred to as time series data), which will be affected by various complicated factors such as economic environment, government policies, and human operation. This paper takes the historical data of stock index as the research object and introduces two models that can be used to make stock index prediction: ARIMA model and LSTM model.
</p>

<p style="text-align:justify">
I first introduce the ARIMA model, which is a classic model in time series analysis. The dataset I am using comes from the Google Finance API, and I have done missing value processing. ARIMA (Auto-Regressive Integrated Moving Average) can be used to predict time series and is often used in demand forecasting and planning. However, if you start with a non-stationary time series, you first need to make a difference until you get a smooth sequence. ARIMA is the most common method in current time series analysis. It is a process of extracting long-term trend, fixed period and other information through differential operation, and transforming non-stationary sequence into the stationary sequence. If $\{x_t\}$ is a $ARIMA(p, d, q)$ model. $d$ means:
$$$$
</p>