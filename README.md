# Principle-Component-Analysis

# PCA Formative Assignment

Principal Component Analysis (PCA) implemented **from scratch with NumPy only** — no sklearn or pandas.

## What this project does

We use PCA to summarise how **30 African countries** (2015–2022) differ in economic performance and population pressure, using World Bank–style indicators.

## Files

| File | Purpose |
|------|---------|
| `Template_PCA_Formative_1.ipynb` | Main notebook — rename with your peer pair number before submitting |
| `data/africa_economic_indicators.csv` | Dataset (14 columns, missing values included) |

## Dataset

- **Non-numeric columns:** `country_name`, `country_iso3`, `region`
- **Numeric columns:** GDP per capita, population, urban/rural %, life expectancy, literacy, CO₂, unemployment, inflation, GDP growth
- **240 rows** (30 countries × 8 years)
- Missing values are filled with each column’s mean before PCA

## How to run

**Google Colab**
1. Upload the notebook and the `data/` folder.
2. Run all cells (`Runtime → Run all`).

**Local**
```bash
pip install numpy jupyter
jupyter notebook Template_PCA_Formative_1.ipynb
```

## Notebook steps

1. Load and clean the data  
2. Standardise features (mean 0, std 1)  
3. Build the covariance matrix  
4. Eigendecomposition → principal components  
5. Select components (≥ 95% variance → 8 components)  
6. Project data and plot before/after PCA  
7. Benchmark vectorised vs loop-based PCA  

## Requirements

- Python 3
- NumPy

