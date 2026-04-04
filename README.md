# BioFinance Pulse 🧬📈
> Analyzing how disease outbreaks impact global stock market sectors

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=flat&logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=flat&logo=jupyter)
![License](https://img.shields.io/badge/License-MIT-green?style=flat)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=flat)

---

## What is this project?

This project investigates the **statistical relationship** between global disease
outbreak data and financial market performance across sectors — healthcare,
pharma, travel, hospitality, and tech.

Using publicly available **WHO disease surveillance data** and **Yahoo Finance
historical prices**, I built a full data pipeline from collection to prediction.

---

## Key Findings

| Disease Event       | Most Impacted Sector | Correlation (r) | Lag (weeks) |
|---------------------|----------------------|-----------------|-------------|
| COVID-19 (2020)     | Travel & Hospitality | -0.87           | 1-2 weeks   |
| COVID-19 (2020)     | Pharma               | +0.74           | 2-3 weeks   |
| H1N1 Influenza      | Healthcare           | +0.61           | 3-4 weeks   |
| Dengue surge (2023) | Insurance            | +0.43           | 2 weeks     |

> Stock markets tend to react 1-3 weeks after outbreak severity escalates.

---

## Project Structure

```
BioFinance-Pulse/
├── notebooks/          # 4 Jupyter notebooks (EDA → ML)
├── src/                # Reusable Python modules
├── data/               # Raw + processed datasets
├── outputs/            # Charts, figures, PDF report
└── dashboard/          # Interactive Plotly Dash app
```

---

## Notebooks Walkthrough

| # | Notebook | What it covers |
|---|----------|---------------|
| 01 | Data Collection | WHO API fetch, Yahoo Finance yfinance pull, merging |
| 02 | Exploratory Analysis | Distribution plots, trend lines, seasonal patterns |
| 03 | Correlation Analysis | Pearson/Spearman correlations, lag analysis, heatmaps |
| 04 | ML Prediction | Random Forest classifier for sector impact prediction |

---

## Sample Visualizations

> *Charts are in `/outputs/figures/` — open the notebooks to see them rendered.*

- Correlation heatmap (disease cases vs sector returns)
- Time-lagged cross-correlation plot
- Sector performance during outbreak timelines
- Feature importance chart (ML model)
- Interactive Plotly dashboard

---

## How to Run

```bash
# 1. Clone the repo
git clone https://github.com/divyanjali123-tyagi/BioFinance-Pulse
cd BioFinance-Pulse

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run notebooks in order
jupyter notebook notebooks/

# 4. Launch interactive dashboard
python dashboard/app.py
```

---

## Tech Stack

- **Data**: `yfinance`, `pandas`, `requests` (WHO API)
- **Analysis**: `numpy`, `scipy`, `statsmodels`
- **Visualization**: `matplotlib`, `seaborn`, `plotly`
- **ML**: `scikit-learn` (Random Forest, cross-validation)
- **Dashboard**: `Dash` by Plotly

---

## About Me

3rd year B.Tech CSE student specializing in **Bioinformatics**.
Passionate about using data to solve real-world problems at the
intersection of biology, health, and technology.

📧 divyanjalityagi4@gmail.com · 💼 https://www.linkedin.com/in/divyanjali-tyagi-a916022b8/ 

---
*Data sources: WHO Disease Outbreak News, Yahoo Finance via yfinance library*
