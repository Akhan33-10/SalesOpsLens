# SalesOpsLens: Sales & Operations MIS (Excel)

An Excel MIS report that gives a sales manager one place to see sales against target, collections, returns and employee performance.

## Business problem
A manager needs daily, weekly and monthly reports they can trust, and a clear view of where to act.

## Data
- 12,000 order records, April to September 2026
- Employee master (50 rows) and product master (20 rows)
- Target_Amount is recorded per order, so achievement % is total sales divided by the sum of order targets

## Data quality
Before reporting, I checked the data and found 7 kinds of issues, listed in an Issue Log with the action taken:
- Duplicate Order ID (2 rows)
- Invalid employee ID
- Invalid product ID
- Missing date
- Negative sale
- Missing target
- Missing region

The 5 rows that would give false totals (the second duplicate, the invalid IDs, the missing date and the negative sale) are excluded with a Valid flag. This leaves 11,995 usable records. The orders with a missing target or missing region are kept, because the sales are real. The order with no region is reported as Unknown.

## What is in the workbook
- Dashboard: KPIs, monthly trend, payment status, sales vs target by region, top and bottom employees, region filter
- Summary: key numbers and the top 3 actions
- Daily, Weekly and Monthly MIS
- Region and Salesperson summaries
- Insights: findings with evidence and action
- Data validation: checks and issue log

All reports use valid rows only and reconcile to the same totals.

## Key numbers
- Sales: Rs 859.0M against order targets of Rs 570.7M (150.5% achievement)
- Collection: 76% of sales value
- Returns: 8% of sales

## Insights
1. Every region and salesperson beat their order targets (regions 147% to 154%, people 137% to 171%). A monthly target per salesperson would be a better basis for judging performance.
2. Regions perform almost the same. The difference is between people.
3. Only 76% of sales value is collected. Pending payments need follow-up.
4. Monthly achievement is flat (144% to 155%), so there is no growth trend.

## Limitations
- Targets are set per order in this data, not per person or per month.
- Employee_Master has a Monthly_Target column, but it adds up to far less than sales, so it is not used.
- The dataset is for practice. The conclusions show the method, not a real business.

## Tools
Excel 2019: SUMIFS, COUNTIFS, INDEX/MATCH, PivotTables, slicers, conditional formatting, data validation.

## Author
Anas Khan | LinkedIn: linkedin.com/in/anas-khan-285415403
