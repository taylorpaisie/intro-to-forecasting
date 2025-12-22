---
layout: default
title: "02 — ETS / ARIMA"
---

## “Real models” (kept lightweight)

For many monthly financial series, ETS (Exponential Smoothing) is a great next step after baselines.

In the notebook we include:
- ETS with optional trend/seasonality
- A simple ARIMA path (optional; depends on your team’s comfort)

## What to watch

- Don’t overfit: if backtest error worsens, step back.
- Beware structural breaks (policy changes, rebaselines, contract transitions).
