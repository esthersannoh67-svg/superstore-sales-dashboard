# Superstore Sales Dashboard

**Practice project using a public sample dataset.**

A small sales dashboard built in Google Sheets from the public "Superstore" sample dataset (orders from 2015 to 2018). I built it to practise pivot tables, charts and KPIs while learning data analytics at BeTechified.

![Superstore Sales Dashboard](Superstore_Dashboard.png)

## Questions I answered

1. How did sales change from year to year?
2. Which product category brings in the most profit?
3. Which region sells the most?
4. Which sub-categories lose money?

## Key numbers

| KPI | Value |
|---|---|
| Total sales | $2,297,201 |
| Total profit | $286,397 |
| Profit margin | 12.47% |
| Number of orders | 5,009 |

## What the data shows

- **Sales grew over the four years.** They dipped slightly in 2016 (about -3%), then rose each year after that. 2018 sales ($733,215) were about 51% higher than 2015 ($484,248).
- **Technology and Office Supplies bring in almost all the profit.** Technology made $145,455 (50.8% of profit) and Office Supplies made $122,491 (42.8%). Furniture made only $18,451 (6.4%), even though it is about a third of all sales, so its profit margin is only about 2.5%.
- **West and East sell the most.** West $725,458, East $678,781, Central $501,240 and South $391,722.
- **Three sub-categories lose money:** Tables (-$17,725), Bookcases (-$3,473) and Supplies (-$1,189). Tables and Bookcases are both in Furniture, which is why that category's profit is so low. I did not look into the reason (for example discounts), so that would be a good next step.

## How I built it

1. Copied the dataset into Google Sheets and cleaned it (see the notes below).
2. Added a helper column, **Year**, with the formula `=YEAR(C2)`.
3. Built four pivot tables (sales by year, profit by category, sales by region, profit by sub-category).
4. Made a chart from each pivot table and gave each a clear title.
5. Calculated the KPIs with `SUM`, `COUNTUNIQUE` and a division for the profit margin.
6. Arranged the KPIs and charts on one Dashboard sheet.

**Tools and skills:** Google Sheets, pivot tables, charts, formulas (`SUM`, `COUNTUNIQUE`, `YEAR`), data cleaning, KPI design.

## Data notes

- The data has 9,994 order lines, which make up 5,009 unique orders. One order can have several products, so I left the repeated order lines as they are.
- The downloaded file had 806 extra rows below the order data (small lookup tables and blank rows). I removed them from my working copy.
- 11 rows have no postal code. They are all Burlington, Vermont, and I left them blank rather than guess.
- The dashboard picture above is from Google Sheets. If you open the Excel file, the charts may look a little different.

## Files in this repository

- `README.md`: this page
- `Superstore_Dashboard.png`: a picture of the finished dashboard
- The Excel workbook: the cleaned data, the four pivot tables and the dashboard

## Author

Esther Sannoh, BeTechified Data Analytics graduate

LinkedIn: linkedin.com/in/esther-sannoh-data-analyst
