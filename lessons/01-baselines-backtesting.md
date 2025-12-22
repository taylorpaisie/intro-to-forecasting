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

We’ll do **rolling-origin** backtesting:
- Train on an initial window
- Forecast the next *h* months
- Slide forward and repeat
