# Objective

The objective of this project is to analyze athletic sales data from two different years (2020 and 2021) using Python within Jupyter Notebook. By visualizing and analyzing the data, we aim to gain insights into various aspects such as regional sales, retailer performance, and product trends.

Jupyter Notebook allows us to interactively explore the data, write and execute Python code, and visualize the results using libraries such as Pandas and Matplotlib. Through this project, we utilize Python's powerful data manipulation and visualization capabilities to derive meaningful insights from the dataset.

# Functionality

1. Combining and Cleaning the Data:
    - concat: We use the pd.concat() function to combine the sales data from 2020 and 2021 into a single DataFrame. This allows us to have a unified dataset for analysis.
    - dtypes: By checking the data types of the columns using .dtypes, we ensure consistency and identify any potential issues with data types.
    - pd.to_datetime: We convert the "invoice_date" column to datetime format using pd.to_datetime(). This makes it easier to perform time-based analysis.

2. Grouping and Aggregating Data:
    - groupby: With the groupby() method, we group the data by specified columns (e.g., region, state, city) and perform aggregations (e.g., sum) on numerical columns (e.g., units_sold, total_sales).
    - agg: The .agg() method is used to specify the aggregation functions (e.g., sum, mean) to apply to each group. This allows us to calculate total sales or total products sold for each group.
    - pivot_table: Using pd.pivot_table(), we pivot the data to create a summary table where rows represent unique combinations of specified columns, and aggregate values are displayed in the cells. This is useful for creating multi-index DataFrames and summarizing data in a structured format.

3. Data Visualization:
    - Matplotlib: We utilize Matplotlib, a popular plotting library in Python, to visualize the data. For example, we can create bar charts or line plots to illustrate sales trends over time or compare performance across regions.
    - Sorting: Sorting the data allows us to identify top-performing regions, retailers, or products easily. We use sorting functions such as .sort_values() to arrange the data in ascending or descending order based on specified columns.

4. Resampling Time Series Data:
    - resample: The resample() function is applied to time series data to change the frequency of the time index. In our project, we use resample() to aggregate daily sales data into weekly or monthly bins, allowing us to analyze sales trends over longer periods efficiently. This helps in identifying weekly or monthly patterns in sales of women's athletic footwear, for example, and understanding seasonal variations in demand.

# Summary

In summary, this project provides valuable insights into athletic sales data, including regional sales performance, retailer profitability, and product trends. By combining, cleaning, and analyzing the data using Python within Jupyter Notebook, we can make informed business decisions and identify areas for improvement.

This analysis can be applied to various real-world scenarios, such as:

- Retail businesses seeking to optimize sales strategies and inventory management.
- Manufacturers looking to understand market demand and consumer preferences.
- Marketing teams aiming to target specific regions or demographics more effectively.
- Investors evaluating the performance of athletic retail companies for potential investment opportunities.