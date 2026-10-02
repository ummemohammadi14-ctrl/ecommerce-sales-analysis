\# E-commerce Sales Analysis \& Product Segmentation



\## Project Overview



This capstone explores product attributes and monthly sales for 1,000 products across 7 categories. The dataset was provided by STAR AGILE for this project.



The project includes exploratory analysis, sales feature engineering, regression model evaluation, and exploratory product profiling with K-Means.



\## Dataset



The dataset has product attributes and 12 monthly sales columns. The project treats their values as sales, but whether they represent units sold, orders, or revenue should be confirmed.



The dataset is included at `data/ecommerce\_sales.csv` and was provided by STAR AGILE for this capstone.



\## Methods



\- Data checks and exploratory analysis with pandas, Matplotlib, and Seaborn

\- Sales feature engineering

\- Linear Regression, Random Forest, tuned Random Forest, and XGBoost

\- Mean-only benchmark with `DummyRegressor`

\- Standardized K-Means clustering with silhouette score evaluation



\## Key Findings



\- Books had the largest sum of recorded sales values by category; Electronics had the highest average sales value per product.

\- The mean-only benchmark achieved an MAE of 775.70. The tested regression models did not meaningfully outperform it.

\- The five-cluster K-Means solution had a silhouette score of about 0.21, indicating overlapping groups. The profiles are exploratory, not confirmed product segments.



\## What This Project Demonstrates



Checked dataset structure, missing values, duplicates, and category coverage.



Created product-level measures from monthly sales, including totals, averages, variability, and Month 1 to Month 12 change.



Compared regression models with both a Linear Regression baseline and a mean-only benchmark.



Used model evaluation results to avoid overstating predictive performance.



Scaled features, profiled K-Means groups, and evaluated cluster separation with the silhouette score.



Translated analysis into business questions while distinguishing observed patterns from proven causes.



\## Business Questions to Investigate



The cluster profiles suggest questions for further analysis—not proven recommendations:



For products with higher recorded sales and review counts, compare profit margins and inventory availability.



For products with high ratings but lower recorded sales, examine website traffic and conversion if that data becomes available.



For products with lower ratings and sales, review customer feedback and profitability before considering product changes.



\## Future Improvements



Confirm whether the monthly sales values represent units, orders, or revenue.



Use dated sales data from multiple years to examine seasonal patterns and evaluate forecasts on future periods.



Add data on inventory, discounts, website visits, conversions, returns, and profit margins.



Check whether the product clusters remain similar when the inputs or cluster count change.



\## Limitations



\- The meaning and business context of the monthly sales values need confirmation.

\- The models did not demonstrate reliable sales prediction with the available features.

\- The clusters overlap and should not be treated as definitive business segments.

\- The data does not include inventory, promotions, website traffic, conversion, or profit margin.

\- The analysis shows patterns in this dataset; it does not prove that product attributes cause sales to change.



\## How to Run


1\. Install the project dependencies listed in `requirements.txt`.

2\. Open notebooks/Ecommerce_Sales_Analysis_&_Product_Segmentation1 (1).ipynb in Jupyter and run the cells in order.
