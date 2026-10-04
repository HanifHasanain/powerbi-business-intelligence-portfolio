# Sales Performance sample dataset

[`sales_performance_sample.csv`](sales_performance_sample.csv) is a fictional 2025 sales dataset for the Sales Performance dashboard preview. It contains 52 records by date and region.

`OrderDate` is the date for each record. `Region` identifies West, Central, East, or South. `Category` identifies the product category. `Revenue` and `Profit` are in USD. `Orders` is the number of orders.

Suggested Power BI measures:

```DAX
Total Revenue = SUM('sales_performance_sample'[Revenue])
Total Profit = SUM('sales_performance_sample'[Profit])
Total Orders = SUM('sales_performance_sample'[Orders])
Profit Margin = DIVIDE([Total Profit], [Total Revenue])
```

The data is fictional and created for this portfolio.

When imported without filters, the data produces the headline values shown in the dashboard preview: **$2.48M revenue**, **$517K profit**, and **12,480 orders**.
