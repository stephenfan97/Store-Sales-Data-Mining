# Store-Sales-Data-Mining

### Exploratory Data Analysis
Exploratory Data Analysis (EDA):

Dataset contains 19,415 rows and 3 columns with no null values.
Analysis includes identifying 164 unique items and 3814 unique members.
Visualizations (bar graphs, pie charts, treemaps) show:
Top 10 most and least frequently purchased items.
Top 10 most frequently visited members.
Monthly sales distribution patterns were observed, revealing insights into item popularity and trends over time.
Dataset Preparation:

Transactions grouped by Member Number and Date to analyze items purchased together.
Used TransactionEncoder for one-hot encoding, converting transactions into a categorical format for analysis.
Methodology:

Applied Apriori and FP-growth algorithms to identify frequent itemsets and generate association rules.
Apriori Algorithm:
Iteratively generates candidate itemsets; requires multiple database scans.
Execution time is higher for large datasets.
FP-growth Algorithm:
Builds an FP-tree to streamline database scans and improve efficiency.
Faster execution compared to Apriori, especially for large datasets.
Parameters:

Minimum support threshold values tested at 0.006, 0.004, and 0.002 to identify frequent itemsets.
Support values of 0.002 yielded meaningful itemsets with at least two items in tuples.
Results and Insights:

Rules characterized by:
Support: Proportion of transactions containing an itemset.
Confidence: Reliability of the rule.
Lift: Likelihood of items being purchased together.
FP-growth demonstrated faster execution with identical results to Apriori.
High-confidence rules highlighted robust item associations, while lift values >1 indicated strong co-purchasing likelihood.
Recommendations:

Optimize product placement by positioning items with strong associations closer together.
Introduce targeted promotions or discounts for commonly paired items.
Leverage insights to enhance the shopping experience and boost sales.
Conclusion:

Both Apriori and FP-growth algorithms are effective in uncovering frequent itemsets and association rules.
FP-growth is recommended for larger datasets due to its efficiency.
Insights from this analysis provide actionable strategies for improving marketing, product placement, and overall customer satisfaction.

### Data Analysis
Refer to attached PDF file & Coding for further information.
