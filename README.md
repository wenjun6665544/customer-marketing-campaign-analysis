# Customer Marketing Campaign Analysis

An Excel-based analysis of customer behavior and campaign response,
with rule-based segmentation to identify audiences for future testing.

## Project Objective

Understand which customer characteristics are associated with campaign
response and develop recommendations for customer targeting.

## Dataset and Cleaning

- Original dataset: 2,240 customer records and 29 variables.
- Retained 2,236 records after excluding three implausible birth years
  and one extreme income value.
- Filled 24 missing income values using the median of the retained records.
- Preserved the original data in a separate worksheet.
- Used 2014 as the reference year for approximate customer age.

## Methods

- Created total spending, purchase count, and historical campaign
  acceptance metrics.
- Compared response rates across spending and age groups.
- Developed rule-based targeting segments using previous campaign
  acceptance, spending, and recency.
- Built an Excel dashboard with formula-driven summaries and charts.

## Key Findings

| Metric | Result |
|---|---:|
| Customers after cleaning | 2,236 |
| Overall campaign response rate | 14.9% |
| High-priority segment size | 238 |
| High-priority segment response rate | 51.7% |
| High-value customer response rate | 28.5% |
| Low-value customer response rate | 8.9% |

The high-priority segment includes customers who accepted at least one
previous campaign and whose most recent purchase was within 50 days
of the observation point.

High-value customers are defined as those with total recorded spending
of at least 1,000; low-value customers spent less than 300.
The currency is not specified in the supplied dataset.

## Recommendations

- Test campaigns with previously engaged, recently active customers.
- Evaluate high-value customers as a second targeting audience.
- Use randomized holdout groups to measure incremental campaign impact.

## Limitations

These are descriptive results from the same sample used to develop the
segments, not validated predictions of future performance.
The 51.7% response rate does not demonstrate a causal improvement.
Data timing and field definitions should be confirmed before deployment.

## Tools

Microsoft Excel: formulas, customer segmentation, tables, and charts.

## Analysis Workbook

[Download the Excel analysis workbook](./marketing_campaign_data_project.xlsx)

The workbook includes a dashboard, customer segmentation analysis,
cleaned data, original data, and a data dictionary.
