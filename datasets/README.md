# Sales Performance sample dataset

[`sales-performance-sample.csv`](sales-performance-sample.csv) is a synthetic 2025 sales dataset for the Sales Performance dashboard preview. It contains 52 sales-summary records at the `OrderDate × Region` grain.

| Column | Description |
| --- | --- |
| `OrderDate` | Date associated with the reporting record |
| `Region` | Sales region: West, Central, East, or South |
| `Category` | Product category associated with the monthly regional record |
| `Revenue` | Sales revenue in USD |
| `Profit` | Profit in USD |
| `Orders` | Number of orders |

Suggested Power BI measures:

```DAX
Total Revenue = SUM('sales-performance-sample'[Revenue])
Total Profit = SUM('sales-performance-sample'[Profit])
Total Orders = SUM('sales-performance-sample'[Orders])
Profit Margin = DIVIDE([Total Profit], [Total Revenue])
```

The dataset is fictional and intended only as a portfolio demonstration.

When imported without filters, the data produces the headline values shown in the dashboard preview: **$2.48M revenue**, **$517K profit**, and **12,480 orders**.
