# Credit Card Transactions SQL Analysis (India)

## 📌 Project Overview
This project explores credit card spending habits in India using SQL Server. The goal is to analyze transaction-level data to uncover insights around city-wise spending, card type trends, gender-based spending patterns, and transaction growth over time.

## 📂 Dataset
- **Source:** [Analyzing Credit Card Spending Habits in India — Kaggle](https://www.kaggle.com/datasets/thedevastator/analyzing-credit-card-spending-habits-in-india)
- **Table name:** `credit_card_transcations`
- **Note:** Column names were converted to lowercase and spaces replaced with underscores before importing into SQL Server. Data types were also corrected on import (the raw file defaults everything to `varchar`).

## 🛠️ Tools Used
- SQL Server (T-SQL)
- Common Table Expressions (CTEs)
- Window Functions (`RANK`, `ROW_NUMBER`, `LAG`, cumulative `SUM`)
- Aggregate & Conditional Aggregation (`CASE WHEN`)

## ❓ Business Questions Solved
1. Top 5 cities with the highest spends and their percentage contribution to total credit card spends
2. Highest spend month and the amount spent in that month, for each card type
3. Transaction details for each card type at the point it crosses a cumulative spend of 1,000,000
4. City with the lowest percentage spend contribution for the Gold card type
5. Highest and lowest expense type per city
6. Percentage contribution of female spends for each expense type
7. Card type & expense type combination with the highest month-over-month growth in Jan 2014
8. City with the highest total-spend-to-transaction-count ratio during weekends
9. City that took the least number of days to reach its 500th transaction (from its first transaction)

## 📁 Repository Structure
```
├── README.md
├── project_solution.sql        -- All SQL queries with solutions
└── sql_project_credit_card_transactions.txt   -- Original problem statement
```

## 🚀 How to Use
1. Download the dataset from the Kaggle link above (or use the provided dataset file).
2. Import it into SQL Server as a table named `credit_card_transcations`, ensuring column names are lowercase with underscores and correct data types are applied.
3. Run the queries in `project_solution.sql` sequentially to reproduce the analysis.

## 📊 Key Insights
- Identified the top-spending cities and their share of overall credit card spend.
- Found seasonal and monthly spending peaks by card type.
- Uncovered gender-based spending patterns across expense categories.
- Highlighted the fastest-growing card/expense type combination in early 2014.
- Determined weekend spending efficiency by city.

## 🔗 Connect
Feel free to explore the queries, raise an issue, or suggest improvements via a pull request.

---
*This project was built as part of a SQL portfolio to demonstrate data exploration and analytical querying skills using window functions, CTEs, and conditional aggregation.*
