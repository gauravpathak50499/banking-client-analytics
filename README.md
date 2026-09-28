# banking-client-analytics
Exploratory data analysis and Power BI dashboard on 3,000 banking clients, covering deposits, loans, and client segments. Built with Python, Pandas, Seaborn, and Power BI.


# Banking Client Analytics: EDA and Power BI Dashboard

Exploratory analysis and an interactive dashboard on a 3,000-client banking dataset, built to understand client segments, deposit behaviour, and loan exposure.

## Overview
The dataset has 25 fields per client, including demographics, income, loyalty tier, banking relationship, deposits, loans, credit cards, and business lending. The goal was to turn raw client records into insights a relationship manager could act on.

## Tools
Python (Pandas, NumPy, Matplotlib, Seaborn) · Power BI · Excel

## What I did
- Cleaned and explored the data (structure, distributions, categorical breakdowns)
- Created income bands (Low / Med / High) for segmentation
- Ran univariate, bivariate, and correlation analysis across 9 financial metrics
- Built a multi-page Power BI dashboard (Summary, Deposit Analysis, Loan Analysis, Q&A) on a star-style data model

## Key findings
- Deposits are strongly correlated with checking (r = 0.84) and savings (r = 0.75) balances, so clients who commit to one account type tend to commit across products
- Loans are about 88% of deposits overall, a useful liquidity and risk indicator
- Business lending is only moderately linked to personal loans (r = 0.44), so it is a distinct client segment
- Private Bank clients are about 45% of the base and hold about 46% of deposits
- Europe accounts for about 43% of total deposits, followed by Asia at about 26%


## Repository structure
- `bankingEDA.ipynb`: analysis notebook
- `Banking.xlsx`: source data (client table plus lookup sheets)
- `Banking Dashboard (2025).pbix`: Power BI report
- `datasets/`: lookup tables (gender, banking relationship, investment advisor)

## How to run
1. Clone the repo
2. Install dependencies: `pip install pandas numpy matplotlib seaborn openpyxl`
3. Open `bankingEDA.ipynb` in Jupyter and run all cells
4. Open the `.pbix` file in Power BI Desktop to explore the dashboard
