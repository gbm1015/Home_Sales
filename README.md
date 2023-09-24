# Home Sales 

## Background

Using our knowledge of SparkSQL to determine key metrics about home sales data.  Followed by using Spark to create temporary views, partition the data, cache and uncache a temporary table, and then verify that the table has been uncached.

The dataset contains information for 33,287 homes, built between 2010-2017, and sold between 2019-2022.  The original dataset can be found at (https://2u-data-curriculum-team.s3.amazonaws.com/dataviz-classroom/v1.2/22-big-data/home_sales_revised.csv).
The dataset has 11 columns including: 
- id, 
- date sold, 
- date built, 
- price, 
- number of bedrooms, 
- number of bathrooms, 
- living space in square footage, 
- lot size in square footage, 
- number of floors,
- whether the house has a waterfront view (yes/no), and
- view rating.

### Before opening the StarterCode folder

1. I created a new repository in GitHub for this project called `Home_Sales`. 
2. Inside the new repository I cloned the new repository to my computer.
3. Inside my local Git repository, I added the starter colab code Home_Sales_starter_code_colab.ipynb.
4. I renamed the starter code from Home_Sales_starter_code_colab.ipynb to Home_Sales_colab.ipynb and uploaded it into Google Colab.
5. I updated the code and completed the requested analysis steps.

## Summary of Analysis Steps

 - Created a Spark Session and read in the home_sales_revised.csv file into a dataframe.
 - Previewed the first 20 rows of the dataframe.
 - Created temporary views of the data.
 - Ran queries on cached and uncached data, and compared the run times.
 - Partitioned the data and leveraged parquet formatted data.
 - Ran queries in Spark to answer the following questions:
     1) What is the average price for a 4 bedroom house sold each year?
     2) What is the average price of a home for each year it was built that has 3 bedrooms and 3 bathrooms?
     3) What is the average price of a home for each year it was built that has 3 bedrooms, 3 bathrooms, 2 floors and is greater than or equal to 2,000 square feet?
     4) What is the "view" rating for homes costing more than or equal to $350,000?
