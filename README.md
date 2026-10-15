# Amazon sales quality checks with pandas

A small Python practice extension to the [e-commerce sales analysis](https://github.com/nour2303/ecommerce-sales-analysis). It uses the first 500 rows from the supplied raw export, with order IDs and address fields removed. The sample is **not representative** of the full dataset.

The [notebook](quality-checks.ipynb) reads the sample, standardizes field names, parses dates and amounts, counts parse failures and duplicate sample rows, and summarizes statuses. It does not claim to reproduce the Power BI report or measure profit.

## Run

Install `requirements.txt`, open the notebook in Jupyter, and run cells from top to bottom. Input is [sample-500-rows.csv](sample-500-rows.csv). The full raw data remains linked from the analytics project.

## Limits

Treat missing amounts, zero quantities, and status labels as business questions, not automatic errors. Do not extrapolate sample totals to the full dataset. This is a practice notebook, separate from the original SQL-cleaning and Power BI analysis.
