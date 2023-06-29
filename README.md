You can see all Insights at the bottom of the Notebook.

Market Analysis and Sales Visualization
This repository contains code that performs market basket analysis and visualizes sales data. The code is written in Python using the pandas and matplotlib libraries.

Data Import
The code begins by importing the necessary libraries and reading the data from three CSV files: order.csv, menu.csv, and detail.csv. The data is loaded into separate pandas DataFrames named df, df1, and df2, respectively.

## Data Merging
The DataFrames are merged into one DataFrame named merged_df using the pd.merge() function. First, df2 is merged with a subset of columns from df1 to include the product information. Then, merged_df is further merged with a subset of columns from df to include the order information. Redundant columns are dropped, and the column name is renamed for clarity.

## Exploratory Data Analysis (EDA)
Market Basket Analysis
The code performs market basket analysis by grouping the merged DataFrame by order_id and creating a list of items for each order. It then calculates the co-occurrence counts for item pairs and identifies the top five item pairs with the highest co-occurrence counts.

## Summing up Sales for Each Day
The code groups the DataFrame by date and calculates the total sales for each day. The daily sales are sorted in descending order, and the DataFrame is displayed.

## Analysis of Revenue
The code provides an overview of revenue statistics, including count, mean, standard deviation, and quartiles. It indicates two specific dates, 2023-05-17 and 2023-03-31, with significantly lower revenue compared to the rest.

## Four Weeks with the Most Revenue
The code calculates the revenue for each week by grouping the DataFrame by week and summing the prices. The weeks are sorted in descending order based on revenue, and the top four weeks with the highest revenue are displayed.

## Average Items per Order
The code calculates the average number of items per order by grouping the DataFrame by order_id and counting the unique product IDs. The average is calculated and displayed.

## Data Visualization
The code includes various visualizations to analyze sales and order trends.

## Revenue per Day
A bar chart is plotted to visualize the revenue per day. The chart is sorted by date and displays the revenue as bars. The x-axis labels are formatted to show dates at a two-week interval for better readability.

## Orders per Day
A line chart is plotted to visualize the number of orders per day over time. The chart shows the trend of orders and uses proper formatting for the x-axis labels to display dates at a two-week interval.

## Revenue by Category
A bar chart is plotted to show the total sales for each category. The chart provides a visual representation of revenue distribution across different categories.

## Best Performing Product
A bar chart is plotted to show the occurrences of each product. The products are sorted based on the count in descending order, and the count is displayed on top of each bar.

## Order Quantity by Category
A bar chart is plotted to show the order quantity for each category. The categories are sorted based on the order quantity in descending order, and the quantity is displayed on top of each bar.

## Average Price per Product in Each Category
The code calculates the average price for each category and prints the results in descending order. This information helps identify the most expensive and least expensive categories.

## Best Performing Day for Each Product
The code calculates the number of orders for each product on a daily basis. It identifies the best performing day for each product based on the highest order count and displays the results.
