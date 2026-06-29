# superstore-sales-analysis
This project analyzes the Superstore dataset to uncover insights on sales, profit, customer behavior, and regional performance using Python (Pandas, Matplotlib, Seaborn). It focuses on identifying loss-making areas, the impact of discounts, and business improvement opportunities.

## Project Overview
This project explores a transactional retail dataset to analyze the relationship between pricing strategy (discounts), shipping modes, geographical performance (states), and overall enterprise profitability.

The data was extracted, comprehensively cleaned, and transformed using Python (Pandas) to uncover key visual correlations, performance drivers, and hidden profit leakages across product segments.

## Tech Stack & Tools
- Language: Python
- Data Manipulation & Analysis: Pandas, NumPy
- Data Visualization: Matplotlib, Seaborn

## Environment: Jupyter Notebook
# Pipeline Phases
1. Data Understanding (Extract)
- Loaded the initial transactional dataset (`sales_analysis.ipynb`) containing structural records of retail shipments.
- Conducted initial statistical summaries and identified missing parameters, datatype anomalies, and redundant operational metrics.

2. Data Cleaning & Feature Engineering (Transform)
- Anomaly Correction: Identified and handled structural values in geospatial markers.
- Handling Redundancies: Identified perfectly duplicated data distributions between tracking variables.
- Feature Engineering: Created calculated fields and categorical metrics for advanced multi-conditional analysis:
  - **Shipping Time (Days):** Calculated as a delta time window ($\text{Ship Date} - \text{Order Date}$) to isolate logistics latency.
  - **Profit Ratio:** Formulated as ($\text{Profit} / \text{Sales}$) to evaluate pure revenue efficiency across various dimensions.
  - **Temporal Extraction:** Parsed time fields into `Order Year` and `Order Month` periods to enable historical trend line tracking.

3. Exploratory Data Analysis (EDA)
- Utilized Seaborn and Matplotlib to construct statistical regression plots, performance rankings, and multi-variable correlation heatmaps.
- Analyzed profit thresholds across distinct subgroups (Product Categories, Sub-Categories, Shipping Classes, and States).

4. Data Aggregation & Value Profiling (Load)
- Summarized localized performance metrics by mapping multi-indexed group metrics into clean aggregate summary frames.
- Segmented transaction distributions against economic frameworks like the 80/20 rule to evaluate revenue distribution risk.

## Key Insights & Findings
- Sales is the Primary Driver but Discount is the Main Killer.
- Aggressive Discounts Drive Net Losses.
- South region has the lowest sales.
- Maximum sales was recorded on 2017-12
- The top 20% of customers contribute 47.96% of the total revenue.
- Shipment mode impact the profit. First class shipment method make the most profit.
- Sub-Category 'Tables' is most affected by the discount.
- Sales is the feature most correlated with Profit, with correlation coefficient of 0.48. As Sales increase, Profit tends to increase as well.

## Files
- sales_analysis.ipynb   — Main EDA notebook and analytical workspace
- superstore.csv         - original dataset from kaggle
- Cleaned_sales_data.csv - cleaned sales data
- requirements.txt       - library that are used in analysis


## 👤 Author
Bikash Sahani
github.com/bikashsahani | linkedin.com/in/bikash-sahani