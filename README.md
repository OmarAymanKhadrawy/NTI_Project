# NTI_Project
# SuperMarket sales 
This dataset contains sales transaction data from a supermarket chain with branches in three major cities: Yangon, Naypyitaw, and Mandalay. The dataset includes information on customer demographics, purchase details, payment methods, and customer satisfaction ratings. Key aspects such as product lines, unit prices, quantities, and total purchase amounts (including tax) are also captured, providing a comprehensive view of sales and customer behavior.


# SuperMarket Sales Project
For our supermarket sales project, we use Python and Power BI to analyze the dataset. In Python, we handle dataset loading, data wrangling, processing, and cleaning. We then use Power BI to create visualizations that highlight valuable insights and uncover hidden relationships, applying a systematic data analysis pipeline throughout the process

## Table of Contents
1. [Introduction](#introduction)
2. [Column Descriptions](#column-descriptions)
3. [Data Analysis](#data-analysis)
4. [Insights](#insights)
5. [Conclusion](#conclusion)

## Introduction
This project explores IMDb data to understand trends in movie ratings and popularity using Excel. It helps identify key patterns in the film industry.

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


## Conclusion

