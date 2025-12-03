# Customer-Shopping-Behaviour
Customer Shopping Behavior Analysis

Overview
End-to-end analysis converting raw Excel customer data into actionable insights and an interactive Power BI dashboard. Built with Excel → Python (Jupyter) → SQL → Power BI.

Tools

Excel (initial import & profiling)

Python (Jupyter, pandas, SQLAlchemy)

Microsoft SQL Server (data warehouse)

Power BI (interactive dashboards)

Quick setup (step-by-step)

Data — Place Customer_Shopping_Behaviour.xlsx in the data/ folder.

Preprocess — Open notebooks/customerBehaviour.ipynb to run data cleaning and feature engineering (fills missing ratings, standardizes categories, removes duplicates/outliers).

Load to SQL — Run notebooks/customerBehaviour.ipynb to push the cleaned table to SQL Server (connection string in .env.example).

Analysis — Use notebooks/customerBehaviour.ipynb to query SQL, perform segmentation, frequency & loyalty calculations, and generate charts.

Dashboard — Open dashboard/Customer Behavior Dashboard.pbix and connect to the SQL database for live visuals (or use exported CSVs in data/ for offline viewing).

Run tests / validation — See notebooks/99_validation.ipynb for data checks and reproducibility steps.

Key outputs

Cleaned dataset (data/cleaned_customers.csv)

SQL script (sql/SQLQuery customer behaviour.sql)

Jupyter notebooks for each pipeline stage

Power BI dashboard highlighting revenue by gender/age, purchase frequency, CLV, shipping & discount behaviours

Presentation file: presentation/Customer Shopping Behaviour Analysis.pptx

Key insights (brief)

Male customers account for the largest revenue share.

Young adults are the top revenue-generating age group.

Loyal customers drive most repeat purchases and CLV.

Express shipping and discount users show higher average spend.

Notes & reproducibility

Store DB credentials in .env (not committed).

Notebooks are linear and reproducible — run 01 → 02 → 03 → 99.

All code is commented and parameterised for easy reuse on larger datasets.
