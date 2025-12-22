---
layout: default
title: "01 — Baselines + backtesting"
---

## Why baselines?

Baselines are your control group. Without them, you can’t tell if your forecast is useful or just… enthusiastic.

## Baselines we’ll use

- **Naive**: forecast = last observed value
- **Seasonal naive**: forecast = value from same month last year
- **Moving average**: forecast = mean of last *k* months

## Backtesting

We'll do **rolling-origin** backtesting (also called "walk-forward" validation):
- Train on an initial window (e.g., months 1–24)
- Forecast the next *h* periods ahead (e.g., *h* = 3 months)
- Calculate error on actual values
- Slide the window forward one period and repeat

This matters because:
- It respects time order (unlike train/test splits)
- It simulates real deployment: you only use past data to forecast future
- It catches models that look good in-sample but fail out-of-sample

## Evaluation metrics

You'll compare baselines using:
- **MAE** (Mean Absolute Error): average forecast error in original units
- **RMSE** (Root Mean Squared Error): penalizes large errors more
- **sMAPE** (Symmetric Mean Absolute Percentage Error): error as % of actual value

Pick one metric for your team and stick with it for consistency.
