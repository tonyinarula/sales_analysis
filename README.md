# Sales Analysis
## Objective

Analyze customer order data to understand revenue drivers, identify top customers, and evaluate purchasing behavior across customer segments and product categories.

## Dataset

The analysis uses two datasets:

* `customers.csv`: customer-level data including customer ID, name, and segment
* `orders.csv`: transactional order data including product, category, quantity, unit price, and order date

The datasets are joined using a customer ID to create a unified, analysis-ready table.

## Tools Used

* **Language:** R
* **Libraries:** tidyverse, lubridate
* **Techniques:** data cleaning, joins, aggregation, cohort analysis, time-based analysis

## Key Questions

* Which customers generate the highest total revenue?
* How does revenue vary across product categories?
* Do different customer segments have different average order values (AOV)?
* How does total revenue change over time on a monthly basis?

## Key Findings

* A small subset of customers contributes a disproportionate share of total revenue, highlighting key accounts
* Revenue is unevenly distributed across product categories, indicating differing product performance
* Certain customer segments exhibit higher average order values than others
* Monthly revenue trends reveal variability over time, useful for identifying seasonality or growth patterns

## Data Cleaning & Assumptions

* Missing order quantities were assumed to represent single-unit purchases
* Order dates were standardized and aggregated to monthly periods for time-based analysis
* Unit prices were imputed using the median price per product to reduce the impact of missing or extreme values
* Revenue calculations assume unit price consistency within each product

## How to Run

1. Clone the repository
2. Ensure `customers.csv` and `orders.csv` are in the working directory
3. Run the R script to generate cleaned data and summary outputs

## Next Steps

* Add customer lifetime value (CLV) calculations
* Perform retention or repeat-purchase analysis
* Visualize monthly revenue trends and segment performance
* Extend analysis with SQL or dashboarding tools for stakeholder use
