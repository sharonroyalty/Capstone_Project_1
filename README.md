# Capstone_Project_1
## Project Title: Capstone Sales Data

## Overview
Sales Data Overview : The sales data contains transaction records for each customer, detailing what items were purchased, the frequency and date of purchases, and customer identifiers. 
This dataset is foundational for analyzing customer behavior, sales trends, and product popularity.

## Data Collected
Here’s a general breakdown of typical fields in sales data:
- CustomerID: Unique identifier for each customer. Used to link purchases to specific individuals for analysis.
- OrderDate: The date and time the purchase was made, allowing for time-based analyses.
- ProductID: Identifier for each product sold, such as shirts, shoes, hats, etc.
- Quantity: Number of units sold in a single transaction.
- Unit Price: Price per unit at the time of sale.
- Revenue: Total cost for the transaction, calculated as Quantity * Price.

## Tools Used
- Microsoft Excel
    - Purpose: Initial data exploration, cleaning, and simple analysis.
    - Usage:Data Cleaning, Pivot Tables, Formulas, Charts
- SQL (Structured Query Language)
    - Purpose: Querying and transforming data in a database, as well as handling large datasets more efficiently than Excel.
    - Usage:Data Extraction,Calculating total sales, average subscription duration, and segment counts by subscription type or customer demographics.
- Power BI
    - Purpose: Advanced data visualization and dynamic reporting for deeper insights into sales and customer trends.
    - Usage: Interactive Dashboards, Calculated Measures, Visualization.
 
## Formulas Used
- Count of Products
  ```EXCEL
   =COUNTIF(Product_Range, Product_Name)

- Revenue
  ```EXCEL
    =Quantity * Price

- Top 5 customers by total purchase amount
  ```SQL
  SELECT TOP 5 
    CustomerID,
    SUM(Revenue) AS TotalPurchaseAmount
  FROM 
    LITA_CAPSTONE PROJECT SALES
   GROUP BY 
    CustomerID, 
  ORDER BY 
    TotalPurchaseAmount DESC;
    ```

  ## Insights and Visualisation
 - Product Performance:
        Identified top-performing products based on total sales, revealing high-revenue items and lower-performing products. Showing that in the year 2023 the product produce more revenue than other but in the year 2024 we see a significant dropdown. These insights can guide inventory planning, promotional focus, and product portfolio adjustments.

 -  Seasonal Sales Trends:
        Observed clear seasonal spikes in sales for certain products. These patterns suggest opportunities to boost marketing efforts and stock levels during peak seasons, maximizing revenue potential.

 -  Revenue Growth:
        Calculated month-over-month and year-over-year growth rates, showing a downward trend in total sales. This positive growth trajectory supports strategic planning for product expansions and market entry.

  Regional Sales Patterns:
        Sales data segmented by region shows specific high-performing areas. We see south stayed as the highest performing region in 2023 and 2024, These insights support targeted regional marketing initiatives and help identify potential new markets for expansion.

![Excel Summary](https://github.com/user-attachments/assets/3c8e8dde-6d51-4642-8334-00af62520b78)
![2024 excel summary](https://github.com/user-attachments/assets/9b444d5a-d9b4-41e8-91f4-92ecc166f8fd)

## Metrics
![Average sales per product](https://github.com/user-attachments/assets/a0c33c6f-cf90-4ea1-8530-041929a4f6a4)
![Revenue by region](https://github.com/user-attachments/assets/a4a9a589-72f5-4700-89ce-711324259674)



  
