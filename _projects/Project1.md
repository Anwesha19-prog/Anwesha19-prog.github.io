---
title: "Immune Risk Model"
excerpt: "A survival prediction model combining clinical + multi-omics signals."
date: 2026-04-10

# Shows a big banner image at the top (hero)
header:
  overlay_image: /assets/images/projects/immune-risk-model/hero.jpg
  overlay_filter: 0.35
  caption: "Figure: Model overview and validation."

# Shows a small thumbnail on the /projects/ grid page
teaser: /assets/images/projects/immune-risk-model/teaser.jpg

# Optional: nice wide layout for projects with images
classes: wide

# If you want a table-of-contents on the right
toc: true
toc_sticky: true
---

## At a glance
| Item | Details |
|---|---|
| What it does | Predicts overall survival risk from clinic + RNA-seq features |
| My role | End-to-end: data curation, modeling, validation, writing |
| Tech | Python, scikit-learn, lifelines, SHAP, pandas |
| Status | Completed |
| Links | [GitHub](https://github.com/YOURUSER/YOURREPO) · [Paper/Preprint](https://example.com) · [Demo](https://example.com) |

## Why this project
Clinicians need interpretable risk estimates. This project explores a model that is both **predictive** and **explainable**, with clear validation strategy.

## Highlights
- Robust preprocessing pipeline (missingness, normalization, leakage checks)
- Nested CV + external validation cohort
- Interpretability with SHAP + feature stability
- Reproducible training with fixed seeds and configs

## Results (put 1–2 key figures)
![ROC / calibration plot]({{ site.baseurl }}/assets/images/projects/immune-risk-model/result1.png)

![Kaplan–Meier stratification]({{ site.baseurl }}/assets/images/projects/immune-risk-model/result2.png)

## How to run
```bash
git clone https://github.com/YOURUSER/YOURREPO
cd YOURREPO
pip install -r requirements.txt
python train.py --config configs/default.yml
