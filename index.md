---
layout: default
title: Intro to Forecasting
---

Welcome! This mini-course is designed for **practical, defensible forecasts** on monthly data (spend, execution, vendor performance, etc.).

## How to use this repo

1. Read the lessons in order:
   - [00 — Course overview](lessons/00-overview.html)
   - [01 — Baselines + backtesting](lessons/01-baselines-backtesting.html)
   - [02 — ETS/ARIMA (lightweight “real models”)](lessons/02-models.html)
   - [03 — Scenarios + communication](lessons/03-scenarios-communication.html)
   - [04 — Capstone](lessons/04-capstone.html)

2. Run the notebook:
   - Notebook file: `notebooks/intro_to_forecasting.ipynb`
   - Recommended: run locally in JupyterLab **or** open in Colab.

### Open in Colab (edit the URL to match your repo)
```text
https://colab.research.google.com/github/<YOUR_GH_USERNAME>/intro-to-forecasting/blob/main/notebooks/intro_to_forecasting.ipynb
```

### View as a static notebook (nbviewer)
```text
https://nbviewer.org/github/<YOUR_GH_USERNAME>/intro-to-forecasting/blob/main/notebooks/intro_to_forecasting.ipynb
```

## What you’ll build

- A baseline forecast (naive / seasonal naive / moving average)
- Rolling backtests + scorecard
- Optional ETS model (if `statsmodels` is installed)
- Scenario forecasts (optimistic / nominal / pessimistic)
- A “tell it to leadership” chart pack (fan chart + key assumptions)
