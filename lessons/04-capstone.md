---
layout: default
title: "04 — Capstone"
---

Build a small forecast “pack” for:
- **Top 5 performers/vendors** by spend (or your highest-impact categories)
- **Total portfolio roll-up** (sum of all groups)

## Deliverables

- **Backtest score table:** MAE/RMSE/sMAPE for each baseline + any model you tried. Show why you picked your final model.
- **6–12 month forecast with interval:** Include your chosen model forecast plus 80% confidence band.
- **3-scenario view:** Nominal, optimistic, pessimistic for 1–3 highest-impact groups.
- **Assumptions log:** 1-page summary of key drivers, macro context, and changes from prior forecast.

## Success criteria

✅ **Your capstone is strong if:**
- Backtest shows your chosen model beats seasonal-naive on holdout data
- Scenarios are internally consistent (same data, different explicit assumptions)
- Assumptions are written for a non-technical stakeholder
- You can explain why you chose your model and why you rejected others

## Common pitfalls to avoid

- **Overfitting:** Just because a model fits history well doesn't mean it will forecast well. Always check backtest error.
- **Inconsistent scenarios:** Don't use different data windows or models for each scenario.
- **Hidden assumptions:** "Optimistic" should *explicitly state* what's different (e.g., "assumes 95% delivery" not just "things go well").
- **Ignoring structural breaks:** If there's a policy change or new contract mid-way, retrain from that point, don't force one model across both regimes.

**Estimated time:** 1–2 hours (with the notebook foundation)
