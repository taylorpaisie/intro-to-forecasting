---
layout: default
title: "00 — Course overview"
---

## Outcomes

By the end, you’ll be able to:

- Forecast monthly series for many groups (e.g., performers/vendors)
- Backtest with rolling-origin evaluation
- Compare models using MAE/RMSE/sMAPE
- Build simple scenarios and communicate uncertainty

## Data shape (recommended)

You can forecast from either:

**A)** long format: `group`, `date`, `value`  
**B)** wide “months as columns” format (common in reporting spreadsheets)

The notebook supports both.

## Ground rules

- Baselines first. If a “fancy model” can’t beat seasonal-naive, it’s not a model—it's a hobby.
- Always backtest.
- Communicate assumptions, not just numbers.
