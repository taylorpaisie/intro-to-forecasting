---
layout: default
title: Intro to Forecasting
---

Welcome! This mini-course is designed for **practical, defensible forecasts** on monthly data (spend, execution, vendor performance, etc.).

**Estimated time:** 2–3 hours (lessons + notebook)  
**Level:** Intermediate (comfortable with Excel/Python)  
**You'll build:** Backtested forecasts, scenarios, and a leadership-ready chart pack

## Quick Start

```bash
# Clone and set up
git clone https://github.com/taylorpaisie/intro-to-forecasting.git
cd intro-to-forecasting

# Create virtual environment (Python 3.8+)
python3 -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter
jupyter lab notebooks/intro_to_forecasting.ipynb
```

**New to this?** Start with [Lesson 00](lessons/00-overview.html) first, then run the notebook.  
**Have data ready?** See [Setup Instructions](#setup-your-data) below.

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
https://colab.research.google.com/github/taylorpaisie/intro-to-forecasting/blob/main/notebooks/intro_to_forecasting.ipynb
```

### View as a static notebook (nbviewer)
```text
https://nbviewer.org/github/taylorpaisie/intro-to-forecasting/blob/main/notebooks/intro_to_forecasting.ipynb
```

## What you’ll build

- A baseline forecast (naive / seasonal naive / moving average)
- Rolling backtests + scorecard
- Optional ETS model (if `statsmodels` is installed)
- Scenario forecasts (optimistic / nominal / pessimistic)
- A “tell it to leadership” chart pack (fan chart + key assumptions)
## Setup Your Data

The notebook supports two data formats:

### Format A: Wide (months as columns)
```
Performer    23-Oct  23-Nov  23-Dec  24-Jan  ...
Alice         1200    1150    1300    1400
Bob           2000    2100    2000    1950
```

### Format B: Long (group, date, value)
```
Performer   Date        Value
Alice       2023-10-01  1200
Alice       2023-11-01  1150
Bob         2023-10-01  2000
...
```

**In the notebook:**
1. Set `DATA_PATH = "path/to/your/data.xlsx"` (or `.csv`)
2. Set `GROUP_COL = "Performer"` (your group column name)
3. For wide format: leave `VALUE_COL = None`
4. For long format: set `DATE_COL` and `VALUE_COL`
5. Run all cells

**Don't have data yet?** Use the [sample data](data/sample_forecast_data.csv) to get familiar with the workflow.

## Troubleshooting

| Problem | Solution |
|---------|----------|
| `FileNotFoundError` | Make sure `DATA_PATH` is correct and file exists |
| No month columns found | Check `MONTH_COL_PATTERN` matches your column headers |
| `NaN` or missing values | Notebook drops rows with missing dates; check source data |
| `statsmodels` errors | Optional; baselines work without it. Install: `pip install statsmodels` |

## Support & Contributing

- Questions? Check the [lessons](lessons/00-overview.html)
- Found a bug? [Open an issue](https://github.com/taylorpaisie/intro-to-forecasting/issues)
- Want to improve? [Pull requests welcome](https://github.com/taylorpaisie/intro-to-forecasting/pulls)