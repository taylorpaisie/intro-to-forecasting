---
layout: default
title: "00 — Course overview"
---

## Why this matters

Forecasting monthly financial or operational data (spend, execution, vendor performance, headcount) is critical for planning, budgeting, and resource allocation. This course teaches you to build **defensible, tested forecasts** that stakeholders can actually trust—not just optimistic projections.

## Outcomes

By the end, you'll be able to:

- Forecast monthly series for many groups (e.g., performers/vendors)
- Backtest with rolling-origin evaluation
- Compare models using MAE/RMSE/sMAPE (Symmetric Mean Absolute Percentage Error)
- Build simple scenarios and communicate uncertainty
- Present forecasts with assumptions clearly documented

**Estimated time:** 2–3 hours (lessons + notebook)

## Data shape (recommended)

You can forecast from either:

**A)** long format: `group`, `date`, `value`  
**B)** wide “months as columns” format (common in reporting spreadsheets)

The notebook supports both.

## Ground rules

- Baselines first. If a “fancy model” can’t beat seasonal-naive, it’s not a model—it's a hobby.
- Always backtest.
- Communicate assumptions, not just numbers.
