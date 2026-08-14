# NSE Stock Portfolio Tracker - Excel Dashboard

![Dashboard Preview](Visuals/dashboard_overview.png)

---

## Project Overview

A personal stock portfolio tracker built entirely in Microsoft Excel, analyzing 28 simulated trades across 8 NSE-listed stocks from January 2022 to October 2023. The project focuses on P&L analysis, win rate, sector performance, holding periods, and cumulative returns over time - built using real historical price data from the NSE Stock Market Historical Dataset on Kaggle.

This is part of my multi-tool data analyst portfolio (Python, SQL, Power BI, Tableau, Excel).

---

## Tools Used

- Microsoft Excel (Structured Tables, Formulas, Conditional Formatting, Dynamic Charts)

---

## Dataset

**Source:** NSE Stock Market Historical Data  
**Platform:** Kaggle (bhaktij)  
**Link:** https://www.kaggle.com/datasets/bhaktij/nse-stock-market-historical-data  

Real historical Open and Close prices were extracted from individual ticker CSVs to simulate realistic buy and sell prices. The trades table was built manually with 28 rows covering 8 NSE-listed stocks across 8 sectors from January 2022 to October 2023.

**Stocks Covered:**

| Ticker | Company | Sector |
|---|---|---|
| RELIANCE.NS | Reliance Industries | Energy |
| TCS.NS | Tata Consultancy Services | IT |
| HDFCBANK.NS | HDFC Bank | Finance |
| INFY.NS | Infosys | IT |
| SUNPHARMA.NS | Sun Pharma | Pharma |
| TATASTEEL.NS | Tata Steel | Metal |
| MARUTI.NS | Maruti Suzuki | Auto |
| ITC.NS | ITC Limited | FMCG |
| ZOMATO.NS | Zomato Limited | Food Tech |

---

## Workbook Structure

| Sheet | Purpose |
|---|---|
| Trades | Raw data - 28 trade records with buy/sell dates, prices, and quantities |
| Analysis | Calculated columns (P&L, Return %, Holding Days, Win/Loss, Month) and all 8 question summary blocks |
| Dashboard | KPI cards and 5 dynamic charts |

---

## Key Questions Answered

1. What is the total portfolio P&L?
2. Which stock has the highest return %?
3. Which sector is most profitable?
4. What is the win rate across all trades?
5. What is the average holding period per stock?
6. Which month had the most trading activity?
7. Which trades had the best risk-reward ratio?
8. What does the cumulative P&L curve look like over time?

---

## Key Excel Features Used

- Structured Tables (Insert > Table) with auto-expanding ranges
- Cross-sheet formula references (Analysis pulling from Trades)
- `SUMIF` / `COUNTIF` / `AVERAGEIF` for grouped aggregations
- `INDEX` / `MATCH` with `MAX` for dynamic winner identification
- `IF` for Win/Loss classification
- `TEXT` function for month label extraction
- Running total formula for cumulative P&L (Q8)
- Conditional Formatting - red/green fill on P&L column
- Data Validation - dropdown list for Sector column
- Dynamic Charts - line, bar, donut, column (all sourced from Analysis summary tables)

---

## Key Findings

- **Total Portfolio P&L: +₹19,734.75** across 28 trades over a 22-month period
- **Win Rate: 53.57%** (15 profitable trades out of 28)
- **FMCG was the most profitable sector** at +₹17,843.50, driven primarily by ITC.NS which had the highest individual return at 15.69%
- **IT was the worst-performing sector** at -₹23,695.35, with INFY.NS losing -12.40% on average across its 4 trades
- **The portfolio was deeply underwater through most of 2022**, recovering sharply in 2023 as MARUTI (+24.9%), ZOMATO (+106.5% on trade 28), and SUNPHARMA (+20.5%) all posted strong exits
- **ZOMATO.NS had the longest average holding period** at 98.5 days, and delivered both the biggest single-trade loss and the biggest single-trade gain in the dataset
- **Most active trading months** were Feb-22, Apr-22, May-22, Jun-22, and Oct-23 - each with 3 trade exits

---

## Dashboard Preview

![Dashboard](Visuals/dashboard_overview.png)

### Cumulative P&L Curve
![P&L Curve](Visuals/pl_curve.png)

### Sector P&L Breakdown
![Sector P&L](Visuals/sector_breakdown.png)

### Top 5 Tickers by Return %
![Top Tickers](Visuals/top_tickers.png)

---

## File Structure

```
stock-portfolio-tracker/
|-- stock_data.xlsx
|-- README.md
|-- Visuals/
    |-- dashboard_overview.png
    |-- pl_curve.png
    |-- sector_breakdown.png
    |-- top_tickers.png
```

---

## Connect

**LinkedIn:** www.linkedin.com/in/pushkesh-m  
**GitHub:** https://github.com/pushkesh-m
