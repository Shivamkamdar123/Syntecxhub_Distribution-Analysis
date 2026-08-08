# Syntecxhub Internship - Project 2
## Statistical Plots & Distribution Analysis

This project is part of the Data Science internship at **Syntecxhub**. It focuses on using `seaborn` to inspect the distribution of numeric data, compare groups, and detect outliers.

## Dataset
Built-in seaborn `tips` dataset — restaurant bill data with columns like `total_bill`, `tip`, `sex`, `day`, `time`, `size`.

## What's in this notebook
- **Histogram + KDE** on `total_bill` and `tip` to check the shape of the distribution
- **Boxplots** comparing `total_bill` across `day` and `time` (Lunch vs Dinner) to see spread and outliers
- **Split violin plot** comparing `total_bill` distribution across `day`, split by `sex`
- **IQR-based outlier detection** — calculated outlier boundaries statistically instead of just reading them off the boxplot
- **Skewness calculation** to quantify how skewed the distributions actually are
- A written interpretation of all the findings at the end

## Key Findings
- `total_bill` is right-skewed (skew ≈ 0.8–1.1 depending on the run) — most bills are low/mid range with a long tail of a few high bills
- Saturday has the highest median bill and the most outliers → weekend spending is higher and more variable
- Dinner bills are higher and more spread out than Lunch bills
- A small number of statistical outliers exist on the high end of `total_bill`, no low-end outliers
- Split violin plot shows male total_bill distribution is slightly wider/higher than female, but both follow the same right-skewed shape

## Folder structure
```
├── project2_distribution_analysis.ipynb   # main notebook
├── outputs/                                # exported plot images (.png)
└── README.md
```

## Tools used
`Python`, `pandas`, `seaborn`, `matplotlib`

## Internship
Syntecxhub | Create · Think · Solve
[www.syntecxhub.com](https://www.syntecxhub.com)
