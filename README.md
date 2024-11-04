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

 -   Regional Sales Patterns:
        Sales data segmented by region shows specific high-performing areas. We see south stayed as the highest performing region in 2023 and 2024, These insights support targeted regional marketing initiatives and help identify potential new markets for expansion.

![Excel Summary](https://github.com/user-attachments/assets/3c8e8dde-6d51-4642-8334-00af62520b78)
![2024 excel summary](https://github.com/user-attachments/assets/9b444d5a-d9b4-41e8-91f4-92ecc166f8fd)

## Metrics
![Average sales per product](https://github.com/user-attachments/assets/a0c33c6f-cf90-4ea1-8530-041929a4f6a4)

-  High and Low-Performing Products:
   Products with a high average sales value indicate premium or high-demand items.
 -  Products with a low average sales are cheaper items or ones that are less popular.
    This helps identify which products are driving more revenue per sale and those that may need better marketing or promotions.

 -  Product Mix Optimization:
   By understanding which products have higher average sales, we can adjust the inventory and focus on stocking items with high profitability, potentially phasing out or reducing stock for low-performing products.

 -   Customer Preferences:
  High average sales for specific products might indicate customer preferences or trends.
    Tracking these insights over time can help forecast demand, adapt to customer trends, and adjust marketing strategies accordingly.
  
  ![Revenue by region](https://github.com/user-attachments/assets/a4a9a589-72f5-4700-89ce-711324259674)
  
- Top-Performing Regions:
    Identify South with the highest revenue, which often indicates strong brand presence, higher demand, or better sales channels.
    These region could be prioritized for additional marketing investment or new product launches.

- Underperforming Regions:
     West Region with low revenue reveal that brand awareness or distribution could be improved.
    Analyzing factors like local competition, pricing differences, or logistical challenges in these regions can help develop targeted strategies to improve sales.

## SQL Queries
- Top 5 total Purchase amount

![Totalpurchaseaount](https://github.com/user-attachments/assets/faa29f10-afc8-4a8c-9d28-564235938c50)

- Total Revenue by Product

![Total Revenue by product](https://github.com/user-attachments/assets/f2ec94b7-25c1-417a-a7d8-fa4568fb97db)

- Popular Subscription

 ![popular subscription](https://github.com/user-attachments/assets/d5a2e32e-b62c-41da-8bdd-6595f94af3e8)

- Percentage of region

![percentage of regional sales](https://github.com/user-attachments/assets/06e2ad61-e1c8-429b-960e-6d874be39d0e)

- Monthly sales amount

![onthlysalestotal](https://github.com/user-attachments/assets/8341aa55-6745-43b3-9938-ea0b3d524282)

- Number of sales Transcation

![Nuber of sales transaction](https://github.com/user-attachments/assets/7d85ca9b-9ba4-4aea-ace8-676199ee0acf)



