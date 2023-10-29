![SparkSQL](https://github.com/afadilla13/Home_Sales/assets/128363337/0591e18e-9edd-453b-995b-ffda4e94b38d)

# Home Sales Analysis with SparkSQL with Google Colab

In this challenge, you'll leverage SparkSQL to extract insights from home sales data. This will involve creating temporary views, partitioning the dataset, caching/un-caching a temporary table, and more.

## Instructions

### 1. Setup
- Rename the `Home_Sales_starter_code.ipynb` file to `Home_Sales.ipynb`.

### 2. Import Dependencies
- Ensure you have the required PySpark SQL functions imported.

### 3. Data Loading
- Load the `home_sales_revised.csv` data from the starter code into a Spark DataFrame.

### 4. Create Temporary Table
- Create a temporary table named `home_sales`.

### 5. Queries
Using SparkSQL, answer the following:
1. Determine the average price for a four-bedroom house sold for each year. Round off your answer to two decimal places.
2. Find the average price of a home for each year it was built that has three bedrooms and three bathrooms. Round off your answer to two decimal places.
3. Ascertain the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet. Round off your answer to two decimal places.
4. Investigate the "view" rating for homes costing more than or equal to $350,000. Determine the run time for this query, and round off your answer to two decimal places.

### 6. Cache Operations
- Cache the `home_sales` temporary table.
- Validate if your temporary table is cached.
- Using the cached data, execute the query that filters out the view ratings with an average price of greater than or equal to $350,000. Measure the runtime and juxtapose it against the uncached runtime.

### 7. Data Partitioning
- Partition the data by the "date_built" field on the formatted parquet home sales data.

### 8. Parquet Temporary Table
- Construct a temporary table for the parquet data.

### 9. Query Performance
- Execute the query that filters out the view ratings with an average price of greater than or equal to $350,000 using the parquet data. Measure the runtime and compare it with the uncached runtime.

### 10. Cleanup
- Uncache the `home_sales` temporary table.
- Confirm that the `home_sales` temporary table has been uncached using PySpark.

### 11. Submission
- Download your `Home_Sales.ipynb` file.
- Upload it into your "Home_Sales" GitHub repository.
