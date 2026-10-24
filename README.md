# Excel PivotTable Basics – Superstore

**Task 24 – Excel PivotTable Basics**
Veda Technology | Data Analytics Track | Level 1, Day 24

## About
I built 3 PivotTables in Excel from the Sample Superstore dataset (2014-2017, 9,994 transactions) to summarize sales by category, region and month, and wrote short insights from them.

## Clean source data
Before building the pivots I checked the source data:
- The data is stored as an Excel Table named `SalesData` (one header row, no blank rows or columns, no merged cells), so the pivots always read the whole table
- Some of the original `Order Date` values were stored as text, so I added a helper column, `Order Date Fixed`, that holds real Excel dates. The monthly pivot uses this column so Excel can group the dates correctly

## The 3 PivotTables
| # | Pivot | Rows | Columns | Values |
|---|-------|------|---------|--------|
| 1 | Sales by category | Category | Year | Sum of Sales |
| 2 | Sales by region | Region | Category | Sum of Sales |
| 3 | Sales by month | Month | Year | Sum of Sales |

## Key results
| Category | Total Sales | Share |
|----------|-------------|-------|
| Technology | 836,154 | 36.4% |
| Furniture | 741,999 | 32.3% |
| Office Supplies | 719,047 | 31.3% |

| Region | Total Sales | Share |
|--------|-------------|-------|
| West | 725,458 | 31.6% |
| East | 678,781 | 29.5% |
| Central | 501,240 | 21.8% |
| South | 391,722 | 17.1% |

| Year | Total Sales |
|------|-------------|
| 2014 | 484,248 |
| 2015 | 470,533 |
| 2016 | 609,206 |
| 2017 | 733,215 |

All three pivots add up to the same grand total of 2,297,201.

## Insights
- **Technology** is the biggest category by sales, but the three categories are close (31% to 36% each)
- **West** is the biggest region and **South** the smallest, which is almost twice as small
- Sales **dipped in 2015** and then grew strongly to 733K in 2017
- Sales are **seasonal**: November 2017 was the highest month (118,448)

## Files
- `PivotTable_Basics.xlsx` – workbook with the Raw Data tab, 3 pivot tabs and an Insights tab
- `pivot_screenshot.png` – screenshot of the pivots
- `README.md`

## Tools used
Microsoft Excel (PivotTables, date grouping)

## Author
Rabia
