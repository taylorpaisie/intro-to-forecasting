---
layout: default
title: "02 — ETS / ARIMA"
---

## “Real models” (kept lightweight)

For many monthly financial series, **ETS** (Error, Trend, Seasonality) is a great next step after baselines. It automatically detects and models trend and seasonal patterns.

**ETS vs. ARIMA:**
- **ETS:** Better for business data with clear trends/seasonality; easier to interpret
- **ARIMA:** More flexible but requires stationarity; harder to explain to non-technical stakeholders

For most monthly spend/execution data, start with ETS.

In the notebook we include:
- ETS with optional trend/seasonality
- A simple ARIMA path (optional; depends on your team's comfort)

## Data requirements

- **Minimum:** 3 years of monthly data (36 observations)
- **Better:** 5+ years (60+ observations) for reliable seasonality detection
- **Watch out:** Structural breaks (policy changes, rebaselines, contract transitions) can invalidate models

## Handling problematic data

- **Missing values:** Interpolate or impute using domain knowledge
- **Outliers/anomalies:** Flag them and consider excluding from training if they're one-time events
- **Sudden structural breaks:** Retrain from the break point forward, or segment the forecast by era

## What to watch

- Don't overfit: if backtest error worsens, step back.
- Always validate: if a "fancy model" doesn't beat seasonal-naive on holdout data, use seasonal-naive.
