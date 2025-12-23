# Intro to Forecasting: Practical Training Kit

A hands-on course for building **backtested, defensible forecasts** on monthly operational data (spend, execution, headcount, vendor performance).

- **5 lessons** on baselines, backtesting, models, and scenarios
- **Runnable notebook** supporting wide and long data formats
- **Sample data** included to get started immediately
- Published as [GitHub Pages](https://taylorpaisie.github.io/intro-to-forecasting/)

## Quick Start

```bash
# Clone and set up (Python 3.8+)
git clone https://github.com/taylorpaisie/intro-to-forecasting.git
cd intro-to-forecasting

python3 -m venv .venv
source .venv/bin/activate           # Windows: .venv\Scripts\activate
pip install -r requirements.txt

# Run the notebook
jupyter lab notebooks/intro_to_forecasting.ipynb
```

**Don't have data yet?** Use `data/sample_forecast_data.csv` to practice the workflow.

## Contents

| Item | Purpose |
|------|---------|
| [Lessons](lessons/) | 5 markdown modules on forecasting theory & practice |
| [Notebook](notebooks/intro_to_forecasting.ipynb) | Interactive template for your data |
| [Sample Data](data/sample_forecast_data.csv) | Learn-by-doing dataset |

## What You'll Learn

✓ Build baseline forecasts (naive, seasonal, moving average)  
✓ Backtest using rolling-origin evaluation  
✓ Compare models with MAE/RMSE/sMAPE  
✓ Create scenario forecasts (optimistic/nominal/pessimistic)  
✓ Present forecasts with assumptions to leadership  

## Customization

To adapt this for your own course:

1. **Rename the repo** in GitHub settings
2. Update `baseurl` in `_config.yml` to `"/<new-repo-name>"`
3. Publish via **Settings → Pages** (choose branch `main`, folder `/ (root)`)
4. Update lesson content in `lessons/`
5. Customize the notebook for your data format in `notebooks/`

## Troubleshooting

- **Lessons not rendering?** Check GitHub Pages settings (may take 1–2 min to deploy)
- **Notebook won't run?** Ensure Python 3.8+, then try: `pip install --upgrade -r requirements.txt`
- **Missing statsmodels?** It's optional; baselines work without it

## License

MIT (feel free to reuse, adapt, and share)
