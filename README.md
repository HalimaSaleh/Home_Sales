# Home_Sales
## Overview

This project involves using Apache Spark to analyze a dataset of home sales. The tasks include reading data, performing various queries, caching, partitioning, and comparing performance.

## Steps

1. **Load Data**: Load the home sales dataset into a Spark DataFrame from a CSV file.
2. **Create Temporary Table**: Create a temporary view of the DataFrame for SQL queries.
3. **Query 1**: Calculate the average price of four-bedroom houses sold per year, rounded to two decimal places.
4. **Query 2**: Calculate the average price of homes with three bedrooms and three bathrooms for each year they were built, rounded to two decimal places.
5. **Query 3**: Calculate the average price of homes with three bedrooms, three bathrooms, two floors, and at least 2,000 square feet, for each year they were built, rounded to two decimal places.
6. **Query 4**: Calculate the average price of homes per "view" rating, with an average price greater than or equal to $350,000, rounded to two decimal places. Measure and print the runtime.
7. **Cache Table**: Cache the `home_sales` temporary table and validate that it is cached.
8. **Cached Query**: Re-run the query from step 6 on the cached table and measure the runtime.
9. **Partition Data**: Partition the dataset by the `date_built` field and save it in Parquet format. Read the partitioned data.
10. **Parquet Table**: Create a temporary table for the parquet data.
11. **Parquet Query**: Re-run the query from step 6 on the parquet table and measure the runtime.
12. **Uncache Table**: Uncache the `home_sales` temporary table and verify it is no longer cached.

## Performance Comparison

Compare the runtimes of queries run on cached data, uncached data, and parquet-formatted data to evaluate performance improvements.

## Notes

- Ensure that Spark and Java are correctly installed and configured.
- The dataset should be properly loaded and formatted for accurate analysis.
- Adjust paths and configurations as needed for your environment.