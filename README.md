# Super Market Sales Project


## Table of Contents
1. [Introduction](#introduction)
2. [Column Descriptions](#column-descriptions)
3. [Data Analysis](#data-analysis)
4. [Insights](#insights)
5. [Conclusion](#conclusion)

## Introduction
This dataset contains sales transaction data from a supermarket chain with branches in three major cities: Yangon, Naypyitaw, and Mandalay. The dataset includes information on customer demographics, purchase details, payment methods, and customer satisfaction ratings. Key aspects such as product lines, unit prices, quantities, and total purchase amounts (including tax) are also captured, providing a comprehensive view of sales and customer behavior.

## Column Descriptions

1. **Invoice ID**  
   A unique identifier for each transaction or purchase.

2. **Branch**  
   Indicates the branch location of the supermarket (e.g., Yangon, Naypyitaw, Mandalay).

3. **Yangon, Naypyitaw, Mandalay**  
   These columns may contain geographical or branch-specific data, though further inspection is needed to clarify their exact role.

4. **Customer type**  
   Describes the type of customer (e.g., Member or Normal).

5. **Gender**  
   Gender of the customer (Male or Female).

6. **Product line**  
   The category or type of product purchased (e.g., Health and beauty, Electronics).

7. **Unit price**  
   The price of a single unit of the product.

8. **Quantity**  
   The number of units purchased in the transaction.

9. **Tax 5%**  
   The tax amount applied to the total purchase (calculated as 5%).

10. **Total**  
    The total amount of the purchase, including tax.

11. **Date**  
    The date of the transaction.

12. **Time**  
    The time the transaction took place.

13. **Payment**  
    The payment method used (e.g., Cash, Credit card, E-wallet).

14. **Rating**  
    The customer satisfaction rating, typically on a scale from 1 to 10.
    

## Data Wrangling, Processing, and Cleaning Steps

1. **Loading the Dataset**  
   - The dataset was loaded into a pandas DataFrame for easy manipulation.

2. **Handling Missing Values**  
   - Checked for missing or null values in columns such as `Branch`, `Gender`, `Product line`, etc. If any missing data were found, they were either imputed (e.g., with mean values for numeric columns or mode for categorical columns) or removed.

3. **Correcting Data Types**  
   - Ensured that data types for each column were appropriate, such as converting `Date` and `Time` to `datetime` objects for easier manipulation and calculations.

4. **Removing Duplicates**  
   - Any duplicate records, if found, were removed to ensure each transaction was unique.

5. **Tax and Total Calculation Check**  
   - Verified that the `Tax 5%` column correctly reflected 5% of the purchase `Total` and fixed any discrepancies in these calculations if needed.

6. **Outlier Detection**  
   - Identified and handled potential outliers in columns like `Unit price`, `Quantity`, and `Rating` that could skew analysis results.

7. **Standardizing Categorical Data**  
   - Ensured consistency in categorical columns such as  `Customer type` by correcting any inconsistencies or misspellings.

8. **Datetime Feature Engineering**  
   - Extracted useful features from the `Date` and `Time` columns, such as day of the week or time of day, for deeper analysis of sales patterns.


## Data Analysis


## Insights

1. *Pie Chart (% Customer Type)*:
   - *Description*: This chart shows the distribution of customer types, comparing the percentage of normal customers versus members. It helps identify the proportion of different customer categories.

2. *Pie Chart (% Customer by Gender)*:
   - *Description*: This visual displays the percentage of customers by gender, highlighting the ratio of male to female customers. It provides insights into the gender demographics of the customer base.

3. *Pie Chart (% Customer by Shift Type)*:
   - *Description*: This chart illustrates the preference of customers for different shift types (first or second shift). It shows which shift is more popular among customers for their purchases.

4. *Stacked Column Chart (Preferred Payment Methods for Customers)*:
   - *Description*: This chart compares different payment methods and shows which method is preferred by customers. The stacked format reveals preferences segmented by customer type.

5. *Stacked Column Chart (Distribution of Customer by Cities)*:
   - *Description*: This visual breaks down the number of customers by city and customer type (normal or member). It helps understand customer distribution across various cities.

6. *Tree Map (Distribution of Product Line by Customers)*:
   - *Description*: This tree map categorizes product lines and shows the number of invoices for each product line. It highlights which product lines are most popular based on customer purchases.

7. *Table Chart (Peak and Low Selling Hours by Product Line)*:
   - *Description*: This table lists each product line along with its peak and low selling hours. It identifies the times of day when products are sold the most and least.

8. *Column Chart (Rating for Products)*:
   - *Description*: This chart displays the count of products based on their rating categories (Good, Fair, Excellent, Very Good). It provides an overview of product ratings and their distribution.

9. *Column Chart (Distribution of Products by Quantity Sold)*:
   - *Description*: This visual compares the total quantity sold for each product line. It shows which product lines have higher or lower sales volumes.

10. *Pie Chart (% Sales for Each City)*:
    - *Description*: This chart represents the percentage of total sales generated by each city. It provides insights into the sales contribution of different cities.

11. *Stacked Column Chart (Distribution of Sales by Product Line Across Shift Types)*:
    - *Description*: This chart compares sales performance for different product lines across various shifts. It shows which product lines achieve higher sales during each shift type.

12. *Line Chart (Average Sales by Hour (10 AM - 9 PM))*:
    - *Description*: This line chart tracks average sales throughout the day from 10 AM to 9 PM. It provides a view of sales trends by hour.

13. *Column Chart (Average Sales Comparison: Weekends vs Weekdays)*:
    - *Description*: This chart compares average sales on weekends versus weekdays. It helps assess the impact of day type on sales performance.

14. *Line Chart (Sales Trend Over 3 Months)*:
    - *Description*: This line chart illustrates the sales trend over the past three months. It provides insights into how sales have fluctuated month by month.

15. *Column Chart (Sales Distribution by Days of Week)*:
    - *Description*: This chart shows sales distribution across different days of the week. It helps identify which days generate higher or lower sales.

## Conclusion

