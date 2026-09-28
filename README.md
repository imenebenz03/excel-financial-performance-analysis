# Financial Performance Analysis Using Excel

## Project Overview

This project analyses financial sales data using Microsoft Excel to evaluate business performance across countries, products, market segments, discount bands, and time periods.

The goal was to practise the workflow of a Data Analyst, from data inspection and validation to financial KPI calculations, PivotTable analysis, data visualisation, and interactive dashboard development.

The final dashboard presents key financial metrics and allows users to explore sales and profitability across different business categories.

## Business Questions

The analysis aimed to answer the following questions:

- How much total sales revenue and profit did the company generate?
- What is the overall profit margin?
- Which countries generate the highest sales and profit?
- Which products contribute the most to financial performance?
- Which market segments generate the highest revenue and profit?
- Are any business segments operating at a loss?
- How does financial performance vary across discount bands?
- How do monthly sales and profit change over time?
- How does performance differ between the available years?

## Dataset

The project uses Microsoft's Financial Sample Excel dataset.

The dataset contains 700 records and 16 original columns covering financial performance across different countries, products, market segments, and discount levels.

The main variables include:

- `Segment`: Business market segment
- `Country`: Country where sales occurred
- `Product`: Product name
- `Discount Band`: Discount classification
- `Units Sold`: Quantity of products sold
- `Manufacturing Price`: Manufacturing price per unit
- `Sale Price`: Selling price per unit
- `Gross Sales`: Revenue before discounts
- `Discounts`: Value of discounts applied
- `Sales`: Revenue after discounts
- `COGS`: Cost of Goods Sold
- `Profit`: Sales minus COGS
- `Date`: Transaction date
- `Month Number`: Numerical month
- `Month Name`: Month name
- `Year`: Transaction year

The available data covers September 2013 to December 2014.

## Tools Used

- Microsoft Excel
- Excel Tables
- Excel formulas
- PivotTables
- PivotCharts
- Slicers

## Data Inspection and Preparation

The project began by inspecting the dataset structure, identifying numerical and categorical variables, and checking data quality.

The following checks were performed:

- Identified 700 records and 16 original columns.
- Reviewed financial, categorical, and date-related variables.
- Used `COUNTBLANK()` to check for missing cells.
- Validated the relationship between Gross Sales, Discounts, and Sales.
- Validated the relationship between Sales, COGS, and Profit.
- Organised the original dataset as an Excel Table named `FinancialData`.

The missing-value check returned zero blank cells.

The financial validation checks also returned zero records flagged as incorrect.

### Financial Calculations

Sales validation:

`Sales = Gross Sales - Discounts`

Profit validation:

`Profit = Sales - COGS`

Profit margin:

`Profit Margin = Total Profit / Total Sales`

The analysis used structured table references, including `SUM(FinancialData[Sales])`, to calculate financial KPIs.

## Financial Performance Summary

The KPI analysis produced the following results:

| KPI | Result |
|---|---:|
| Total Sales | $118,726,350.26 |
| Total Profit | $16,893,702.26 |
| Total COGS | $101,832,648.00 |
| Total Discounts | $9,205,248.24 |
| Profit Margin | 14.23% |

The company generated approximately $118.73M in sales and $16.89M in profit.

An overall profit margin of 14.23% means that approximately $14.23 in profit was generated for every $100 of sales.

## Exploratory Data Analysis

### Sales by Country

A PivotTable was created to calculate total sales by country.

| Country | Total Sales |
|---|---:|
| United States of America | $25.03M |
| Canada | $24.89M |
| France | $24.35M |
| Germany | $23.51M |
| Mexico | $20.95M |

The United States generated the highest sales, followed closely by Canada and France.

The difference between the highest and lowest sales markets was relatively modest compared with some of the differences observed in profitability.

### Profit by Country

A separate PivotTable was created to analyse total profit by country.

| Country | Total Profit |
|---|---:|
| France | $3.78M |
| Germany | $3.68M |
| Canada | $3.53M |
| United States of America | $3.00M |
| Mexico | $2.91M |

France generated the highest total profit despite not having the highest sales.

The United States generated the highest sales but ranked fourth in total profit.

This demonstrates why revenue and profit should be examined together when evaluating financial performance.

### Product Performance

Sales, profit, and units sold were analysed for each product.

| Product | Total Sales | Total Profit |
|---|---:|---:|
| Paseo | $33.01M | $4.80M |
| VTT | $20.51M | $3.03M |
| Velo | $18.25M | $2.31M |
| Amarilla | $17.75M | $2.81M |
| Montana | $15.39M | $2.11M |
| Carretera | $13.82M | $1.83M |

Paseo generated the highest sales and profit, making it the largest overall contributor to financial performance among the six products.

VTT generated the second-highest sales and profit.

Amarilla generated less sales than Velo but achieved higher total profit, demonstrating that sales rankings and profit rankings do not necessarily follow the same order.

### Business Segment Performance

Sales and profit were analysed across five business segments.

| Segment | Total Sales | Total Profit |
|---|---:|---:|
| Government | $52.50M | $11.39M |
| Small Business | $42.43M | $4.14M |
| Enterprise | $19.61M | -$0.61M |
| Midmarket | $2.38M | $0.66M |
| Channel Partners | $1.80M | $1.32M |

Government generated the highest sales and profit, making it the largest contributor to overall business performance.

Small Business generated the second-highest sales and profit.

The Enterprise segment generated approximately $19.61M in sales but recorded a loss of approximately $614,546.

This is an important finding because it shows that generating substantial revenue does not necessarily translate into profitability.

### Discount Band Analysis

Financial performance was compared across four discount bands.

| Discount Band | Total Sales | Total Discounts | Total Profit |
|---|---:|---:|---:|
| High | $37.37M | $5.32M | $3.39M |
| Medium | $38.78M | $3.00M | $5.58M |
| Low | $34.63M | $0.89M | $6.19M |
| None | $7.94M | $0.00M | $1.74M |

The Medium discount band generated the highest total sales at approximately $38.78M.

However, the Low discount band generated the highest total profit at approximately $6.19M.

The High discount band recorded the largest discount value, approximately $5.32M, but generated less profit than both the Low and Medium discount bands.

These results suggest that discount strategies should be investigated further. However, the analysis does not establish that discounts directly caused differences in profit, as sales volumes, product mix, and costs may also influence the results.

### Monthly Financial Performance

Sales and profit were analysed by month using PivotTables and a line chart.

The monthly analysis covered September 2013 to December 2014.

The results showed noticeable fluctuations in sales and profit throughout the available period.

October 2014 recorded the highest monthly sales at approximately $12.38M.

December 2014 also recorded strong performance, generating approximately $12.00M in sales and $2.03M in profit.

The monthly chart made it possible to compare sales and profit trends across both years.

### Annual Financial Performance

Sales and profit were aggregated by year.

| Year | Total Sales | Total Profit |
|---|---:|---:|
| 2013 | $26.42M | $3.88M |
| 2014 | $92.31M | $13.02M |

2014 recorded substantially higher total sales and profit than 2013.

However, the dataset contains only September to December for 2013, whereas 2014 contains a complete year.

Therefore, the annual totals are not directly comparable as measures of year-over-year growth.

## Dashboard Development

An Excel dashboard was developed to communicate the financial results through KPIs and visualisations.

The dashboard includes four financial KPI cards:

- Total Sales
- Total Profit
- Profit Margin
- Total Discounts

The visualisations include:

- Total Sales by Country
- Total Profit by Country
- Sales vs Profit by Product
- Sales vs Profit by Segment
- Sales and Profit by Discount Band
- Monthly Sales and Profit Trend

An additional annual performance chart was created on the yearly analysis worksheet.

Country and Segment slicers were added to support interactive exploration of the PivotTable results.

A supporting PivotTable was also created to retrieve filtered financial totals, allowing KPI calculations to be linked to dashboard selections.

## Key Business Insights

- The company generated approximately **$118.73M in sales and $16.89M in profit**, achieving an overall profit margin of **14.23%**.

- The United States generated the highest sales at approximately **$25.03M**, while France generated the highest profit at approximately **$3.78M**. This demonstrates that the market with the highest revenue is not necessarily the most profitable.

- Paseo was the strongest-performing product in absolute financial terms, generating approximately **$33.01M in sales and $4.80M in profit**.

- Government was the largest business segment, contributing approximately **$52.50M in sales and $11.39M in profit**.

- The Enterprise segment recorded a loss of approximately **$614,546** despite generating $19.61M in sales. Its financial performance requires further investigation.

- The Low discount band generated the highest total profit at approximately **$6.19M**, while the Medium discount band generated the highest sales at approximately **$38.78M**.

- The High discount band recorded approximately **$5.32M in discounts**, but its total profit was lower than both the Low and Medium discount bands.

- Monthly financial performance fluctuated throughout the available period, with particularly strong sales in October and December 2014.

## Business Recommendations

- Investigate the Enterprise segment to understand why it generates a loss despite its substantial sales revenue. Further analysis should examine product mix, costs, pricing, and discount levels within this segment.

- Monitor product-level profitability rather than relying exclusively on sales rankings. Paseo should receive particular attention because of its significant contribution to total sales and profit.

- Review discount effectiveness across products and segments. The Low discount band generated the highest total profit, suggesting that the relationship between discount levels and profitability deserves further investigation.

- Compare revenue and profitability when evaluating geographic markets. The United States leads in sales, but France and Germany generate higher total profit.

- Continue monitoring Government and Small Business performance because these segments contribute the majority of the company's total sales and profit.

- Use monthly financial monitoring to identify unusual increases or decreases in sales and profit and support more informed operational planning.

- Obtain additional comparable time periods before drawing conclusions about annual growth or recurring seasonal patterns.

## Skills Demonstrated

- Inspecting Excel datasets
- Identifying categorical and numerical variables
- Checking missing values using `COUNTBLANK()`
- Validating financial calculations using `IF()`
- Counting failed checks using `COUNTIF()`
- Working with Excel Tables
- Using structured table references
- Calculating financial KPIs using `SUM()`
- Calculating profit margins
- Handling formula errors using `IFERROR()`
- Creating PivotTables
- Aggregating sales, profit, costs, and discounts
- Creating PivotCharts
- Using clustered bar and column charts
- Creating monthly line charts
- Grouping dates by month and year
- Sorting aggregated results
- Creating dashboard KPI cards
- Adding interactive slicers
- Connecting slicers to multiple PivotTables
- Creating dynamic financial summaries
- Comparing revenue and profitability
- Identifying loss-making business segments
- Interpreting financial trends
- Writing business insights
- Developing data-driven recommendations

## Conclusion

This project demonstrated how Excel can be used to transform financial transaction data into meaningful business information.

The analysis identified important differences between sales and profitability across products, countries, segments, and discount bands.

In particular, the Enterprise segment's negative profit and the differences between country sales and profit rankings highlighted the importance of analysing financial performance beyond revenue alone.

The completed project brings together data validation, financial analysis, PivotTables, data visualisation, and dashboard development in an end-to-end Excel portfolio project.