# DSCI 552 — Homework 5

Jesse Ngo

Decision trees as interpretable models on the UCI Acute Inflammations data (label powerset tree, IF-THEN rules, cost-complexity pruning), and regression on the UCI Communities and Crime data: median imputation, correlation matrix, coefficient of variation, least squares, ridge, the LASSO (raw and standardized features), PCR, and an L1-penalized gradient boosting tree with XGBoost.

## Structure

```
.
├── README.md
├── .gitignore
├── requirements.txt
├── data
│   ├── diagnosis.data / diagnosis.names        (Acute Inflammations)
│   └── communities.data / communities.names    (Communities and Crime)
└── notebook
    └── Ngo_Jesse_HW5.ipynb
```

## Running

```
pip install -r requirements.txt
```

Open `notebook/Ngo_Jesse_HW5.ipynb` in Jupyter and run all cells (a couple of minutes; the PCR grid search and the XGBoost cross-validation are the slow parts). The data is loaded with the relative path `../data`. `diagnosis.data` is UTF-16 encoded with comma decimals and is read with those options; no data files were edited.

## Data

- Acute Inflammations, UCI Machine Learning Repository: https://archive.ics.uci.edu/ml/datasets/Acute+Inflammations
- Communities and Crime, UCI Machine Learning Repository: https://archive.ics.uci.edu/ml/datasets/Communities+and+Crime
