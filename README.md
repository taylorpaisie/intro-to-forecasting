# Intro to Forecasting (GitHub Pages + Notebook)

This repo is a starter kit for an **Intro to Forecasting** training:
- Markdown lessons published via **GitHub Pages**
- A runnable **Jupyter notebook** for hands-on analysis

## Run the notebook locally

```bash
python -m venv .venv
# Windows: .venv\Scripts\activate
source .venv/bin/activate

pip install -r requirements.txt
jupyter lab
```

Open: `notebooks/intro_to_forecasting.ipynb`

## Publish the lessons with GitHub Pages

In your repo:
1. Go to **Settings → Pages**
2. Select **Deploy from a branch** (simple) or **GitHub Actions** (more control)
3. Choose branch `main` and folder `/ (root)`

If you rename the repo, update `baseurl` in `_config.yml`.
