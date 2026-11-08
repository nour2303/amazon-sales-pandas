# E-Commerce Data Quality Checks with Python & pandas

A Python and **pandas** data quality profiling workflow built as a companion to the [E-Commerce Sales Analysis](https://github.com/nour2303/ecommerce-sales-analysis) project.

The Jupyter notebook ([`quality-checks.ipynb`](quality-checks.ipynb)) demonstrates a repeatable Python workflow for auditing raw e-commerce CSV exports before loading them into a database or BI tool:

- **Schema Standardization:** Normalizes column names and strips whitespace across raw text fields.
- **Type Parsing & Validation:** Parses order dates and numeric currency amounts while flagging unparseable or missing values.
- **Deduplication Checks:** Identifies exact duplicate rows and summarizes record counts before and after cleaning.
- **Order Status Profiling:** Generates summary tables across completed, cancelled, and returned order statuses.

## Getting Started

1. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
2. Open [`quality-checks.ipynb`](quality-checks.ipynb) in Jupyter Notebook or VS Code and run all cells against the included [`sample-500-rows.csv`](sample-500-rows.csv) dataset (or point the file path to the full e-commerce CSV extract).
