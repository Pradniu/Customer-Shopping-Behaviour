# Customer-Shopping-Behaviour-Analysis

<img width="900" height="500" alt="image" src="https://github.com/user-attachments/assets/0c82bdf9-09e8-41f2-9997-bbba1c4d4de5" />

## Table of Contents
- [Overview](#overview)
- [Business Problem](#business-problem)
- [Technologies](#technologies)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Project Workflow](#project-workflow)
- [Key Insights](#key-insights)
- [Business Recommendations](#business-recommendations)
- [Methodology](#methodology)
- [Notes & Reproducibility](#notes--reproducibility)
- [Conclusion](#conclusion)

## Overview

This project is an end-to-end analysis of customer shopping behaviour, starting from raw Excel data and transforming it into actionable business insights and an interactive Power BI dashboard.

The goal was not just to analyse the data, but to understand who the most valuable customers are and how businesses can use this information to improve revenue and customer retention.

**Pipeline:** Excel → Python (Jupyter) → SQL Server → Power BI

## Business Problem

Retail businesses often collect large amounts of customer data but struggle to turn it into meaningful decisions.

This project focuses on:
- Identifying high-value customers
- Understanding purchasing patterns
- Finding opportunities to improve revenue and engagement

<img width="900" height="500" alt="image" src="https://github.com/user-attachments/assets/59265677-2543-4604-9fab-ff73fc00afb3" />

## Technologies

- **Excel** — Initial data profiling and validation
- **Python** — ETL and statistical analysis (Jupyter, pandas, SQLAlchemy)
- **Microsoft SQL Server** — Data warehouse and complex queries
- **Power BI** — Interactive visualization and KPI tracking

## Project Structure

```
├── data/
│   ├── raw/                         # Original Excel file
│   └── processed/                   # Cleaned data
├── notebooks/
│   ├── 01_data_preparation.ipynb   # Data cleaning & validation
│   ├── 02_transformation.ipynb     # ETL to SQL Server
│   ├── 03_analysis.ipynb           # Customer & revenue analysis
│   └── 99_utilities.ipynb          # Helper functions & reusable code
├── dashboards/
│   └── customer_analysis.pbix      # Power BI interactive dashboard
├── .env.example                    # Template for database credentials
├── requirements.txt                # Python dependencies
└── README.md
```

## Getting Started

### Prerequisites
- Python 3.8+
- Microsoft SQL Server (local or Azure)
- Power BI Desktop
- Git

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Pradniu/Customer-Shopping-Behaviour.git
   cd Customer-Shopping-Behaviour
   ```

2. Create a virtual environment and install dependencies:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```

3. Configure database credentials:
   ```bash
   cp .env.example .env
   # Edit .env with your SQL Server connection details
   ```

4. Run notebooks in sequence:
   - `01_data_preparation.ipynb` — Clean and validate raw data
   - `02_transformation.ipynb` — Load data into SQL Server
   - `03_analysis.ipynb` — Generate insights and metrics
   - `99_utilities.ipynb` — Optional: explore helper functions

5. Open Power BI Dashboard:
   - Launch Power BI Desktop
   - Open `dashboards/customer_analysis.pbix`
   - Connect to your SQL Server instance

## Project Workflow

### 1. Data Preparation
- Imported raw Excel dataset
- Cleaned missing values and handled inconsistencies
- Standardised categories and removed duplicates

### 2. Data Transformation & Storage
- Loaded cleaned data into SQL Server
- Structured data for efficient querying and aggregation

### 3. Analysis
- Analysed customer demographics and purchase behaviour
- Calculated purchase frequency and customer loyalty metrics
- Explored relationships between discounts, shipping, and spending

### 4. Visualisation
- Built an interactive Power BI dashboard
- Visualised revenue trends, customer segments, and purchasing patterns

<img width="900" height="500" alt="image" src="https://github.com/user-attachments/assets/ffcc4af9-b9da-48fa-8198-dd5ecdff96e0" />

## Key Insights

- **Male customers** contributed a larger share of overall revenue
- **Young adult customers** were the most active and highest spending segment
- **A small group of loyal customers** generated a significant portion of repeat purchases
- **Customers using express shipping and discounts** tended to spend more
- **Peak spending months** identified for seasonal campaign planning

## Business Recommendations

1. **Focus marketing efforts** on high-spending customer segments → Expected ROI: Increased engagement by 20-30%
2. **Introduce loyalty programs** to retain repeat customers → Increase retention by 15%+
3. **Promote high-performing product categories** to maximise revenue → Quick win for Q3-Q4
4. **Use targeted discounts strategically** to increase engagement without eroding margins

<img width="900" height="500" alt="image" src="https://github.com/user-attachments/assets/901540be-7c32-4d4a-8197-818aee104338" />

## Methodology

- **RFM Analysis** (Recency, Frequency, Monetary) — Segmented customers into actionable groups
- **Statistical Testing** — Validated relationships between variables (discounts, shipping, spending)
- **Data Normalisation** — Ensured accurate trend analysis across different scales
- **Cohort Analysis** — Tracked customer behaviour over time by acquisition period

## Notes & Reproducibility

- **DB Credentials** — Store sensitive data in `.env` (never commit credentials)
- **Linear Workflow** — Notebooks are reproducible — run in order: `01 → 02 → 03 → 99`
- **Parameterised Code** — All code is commented and parameterised for easy reuse on larger datasets
- **Idempotent Scripts** — Safe to re-run without data duplication

## Conclusion

This project demonstrates how raw customer data can be transformed into meaningful insights that support business decisions.

It highlights my ability to work across the full data pipeline and connect technical analysis with real-world outcomes.

---

**Questions or feedback?** Feel free to open an issue or reach out!
