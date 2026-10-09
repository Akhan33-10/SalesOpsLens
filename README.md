# SalesOpsLens: Sales & Operations MIS (Excel)

An Excel MIS report that gives a sales manager one place to see sales against target, collections, returns and employee performance.

## Business problem
A manager needs daily, weekly and monthly reports they can trust, and a clear view of where to act.

## Data
- 12,000 order records, April to September 2026
- Employee master (50 rows) and product master (20 rows)

## Data quality
Before reporting, I checked the data and found 5 problem rows: a duplicate Order ID, an invalid employee ID, an invalid product ID, a missing date and a negative sale. I also found one order with a missing region. Each issue is logged with the action taken. The 5 problem rows are excluded using a Valid flag, which leaves 11,995 usable records. The order with no region is kept and reported as Unknown, because the sale is real.

## What is in the workbook
- Dashboard: KPIs, trend, payment status, sales vs target by region, top and bottom employees, region filter
- Summary: key numbers and the top 3 actions
- Daily, Weekly and Monthly MIS
- Region and Salesperson summaries
- Insights: findings with evidence and action
- Data validation: checks and issue log

## Key numbers
- Sales: Rs 859.0M against a target of Rs 570.7M (151% achievement)
- Collection: 76% of sales value
- Returns: 8% of sales

## Insights
1. Every region and every salesperson beat target (regions 147% to 154%, people 137% to 171%). Targets may be too low.
2. Regions perform almost the same. The difference is between people.
3. Only 76% of sales value is collected. Pending payments need follow-up.
4. Monthly achievement is flat (144% to 155%), so there is no growth trend.

## Tools
Excel 2019: SUMIFS, COUNTIFS, INDEX/MATCH, PivotTables, slicers, conditional formatting, data validation.

## Author
Anas Khan | LinkedIn: linkedin.com/in/anas-khan-285415403
