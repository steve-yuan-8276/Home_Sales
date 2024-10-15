# Home Sales Analysis Using SparkSQL

## Project Overview

The goal of this project is to explore and analyze home sales data using PySpark and SparkSQL, leveraging features like caching, partitioning, and temporary tables to improve data processing efficiency.

## Files

This project runs in a local environment; please refer to Home_Sales.ipynb for specific details.

## Instructions

1. **Rename the File**: Rename the `Home_Sales_starter_code.ipynb` file to `Home_Sales.ipynb`.

2. **Import Spark Functions**: Import the necessary PySpark SQL functions for this assignment.

3. **Read Home Sales Data**: Load the `home_sales_revised.csv` data into a Spark DataFrame.

4. **Create Temporary Table**: Create a temporary table called `home_sales` for querying.

5. **Answer Questions Using SparkSQL**:

    - **Average Price of Four-Bedroom Houses**: Determine the average price for four-bedroom homes sold for each year. Round the answer to two decimal places.

    - **Average Price for Homes with 3 Bedrooms and 3 Bathrooms**: Calculate the average price of homes with 3 bedrooms and 3 bathrooms for each year they were built. Round the answer to two decimal places.

    - **Average Price for Specific Criteria**: Calculate the average price of homes with 3 bedrooms, 3 bathrooms, 2 floors, and a square footage greater than or equal to 2,000 sq. ft. for each year they were built. Round to two decimal places.

    - **Average Price by "View" Rating**: Determine the average price of homes by "view" rating where the average home price is greater than or equal to $350,000. Record the runtime and round the answer to two decimal places.

6. **Caching**:

    - Cache the `home_sales` temporary table.

    - Verify that the `home_sales` table is cached.

7. **Run Query on Cached Data**: Execute the query from step 5 (average price by "view" rating) on the cached data and compare the runtime to the uncached version.

8. **Partition Data**: Partition the home sales data by the `date_built` field and save it in Parquet format.

9. **Create Parquet Table**: Create a temporary table from the partitioned Parquet data.

10. **Run Query on Parquet Data**: Execute the query from step 5 on the partitioned Parquet data and compare the runtime to the uncached version.

11. **Uncache Table**: Uncache the `home_sales` temporary table.

12. **Verify Uncaching**: Verify that the `home_sales` table has been uncached.

Thanks for your time.