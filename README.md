# Data Vortex — Round 1 Phase 1 notebook

Use `DataVortexEDAR1.ipynb` to clean the recovered intake data and run EDA.

The repo also contains the EDA report as FinalReportR1.pdf

## Open

Google Colab or Jupyter (Python 3). Required packages: `pandas`, `numpy`, `matplotlib`.

Colab already has these. Locally:

```
pip install pandas numpy matplotlib
```

Open the notebook and **Run all**.

## How it works

Raw CSVs are embedded in the notebook (`StringIO`). You do not need `db1.csv` / `db2.csv` on disk.

- `df2` = posts
- `df1` = users

Sections: inspect, duplicates/anomalies, clean, distributions, time/engagement, platform stats, correlation, export.

## Output

The last cell writes to the current working directory:

- `df2_cleaned.csv`
- `df1_cleaned.csv`
- `Final_dataset.csv`

This folder also includes the cleaned tables used for submission (`dataset1_cleaned_posts.csv`, `dataset2_cleaned_users.csv`, `Final_dataset.csv`).
