# Customer-Shopping-Behaviour-Analysis

<img width="900" height="500" alt="image" src="https://github.com/user-attachments/assets/0c82bdf9-09e8-41f2-9997-bbba1c4d4de5" />


Overview

This project is an end-to-end analysis of customer shopping behaviour, starting from raw Excel data and transforming it into actionable business insights and an interactive Power BI dashboard.

The goal was not just to analyse the data, but to understand who the most valuable customers are and how businesses can use this information to improve revenue and customer retention.

Pipeline: Excel → Python (Jupyter) → SQL Server → Power BI

Business Problem

Retail businesses often collect large amounts of customer data but struggle to turn it into meaningful decisions.

This project focuses on:

Identifying high-value customers

Understanding purchasing patterns

Finding opportunities to improve revenue and engagement

Tools

Excel (initial import & profiling)

Python (Jupyter, pandas, SQLAlchemy)

Microsoft SQL Server (data warehouse)

Power BI (interactive dashboards)

<img width="900" height="500" alt="image" src="https://github.com/user-attachments/assets/59265677-2543-4604-9fab-ff73fc00afb3" />

Project Workflow

1. Data Preparation

Imported raw Excel dataset
Cleaned missing values and handled inconsistencies
Standardised categories and removed duplicates

2. Data Transformation & Storage

Loaded cleaned data into SQL Server
Structured data for efficient querying

3. Analysis

Analysed customer demographics and purchase behaviour
Calculated purchase frequency and customer loyalty
Explored relationships between discounts, shipping, and spending

4. Visualisation

Built an interactive Power BI dashboard
Visualised revenue trends, customer segments, and purchasing patterns

Key Insights

Male customers contributed a larger share of overall revenue

Young adult customers were the most active and highest spending segment

A small group of loyal customers generated a significant portion of repeat purchases

Customers using express shipping and discounts tended to spend more

<img width="900" height="500" alt="image" src="https://github.com/user-attachments/assets/ffcc4af9-b9da-48fa-8198-dd5ecdff96e0" />


Business Recommendations

Focus marketing efforts on high-spending customer segments

Introduce loyalty programs to retain repeat customers

Promote high-performing product categories to maximise revenue

Use targeted discounts strategically to increase engagement

<img width="900" height="500" alt="image" src="https://github.com/user-attachments/assets/901540be-7c32-4d4a-8197-818aee104338" />


Notes & reproducibility

Store DB credentials in .env (not committed).

Notebooks are linear and reproducible — run 01 → 02 → 03 → 99.

All code is commented and parameterised for easy reuse on larger datasets.

Conclusion

This project demonstrates how raw customer data can be transformed into meaningful insights that support business decisions.

It highlights my ability to work across the full data pipeline and connect technical analysis with real-world outcomes.
