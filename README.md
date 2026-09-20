SUNRISE SUPERMARKET SQL ASSIGNMENT ONE

STUDENT INFORMATION

Name:Mutesi Liza Phiona  
Student ID: 29793  
DBMS: Oracle Database

PROJECT SUMMARY

This project is a SQL database system for Sunrise Supermarket.
It manages customers, products, orders, and order items and uses SQL queries to analyze customer spending and sales information.

BUSINESS SCENARIO

Sunrise Supermarket needs a database to manage customer information, products, orders, and sales. 
The database helps the supermarket track purchases, calculate customer spending, rank customers, and analyze revenue over time.

 DATABASE TABLES

The database contains the following tables:

- CUSTOMERS – stores customer information.
- PRODUCTS– stores product names, categories, and prices.
- ORDERS – stores customer orders and order dates.
- ORDER_ITEMS – stores the products and quantities included in each order.

 DATA POPULATION

The database contains:

- 5 customers
- 8 products
- 15 orders
- 25 order items
- Products from at least 3 categories
- Orders recorded across multiple dates

 REQUIRED SQL QUERIES

JOIN 1 – ORDERS AND CUSTOMERS

Lists every order together with the customer's name, city, and order date.
The INNER JOIN connects the orders table with the customers table using customer_id.
It shows the order ID, customer's name, city and order date. Only orders that have a matching customer are displayed

Business Interpretation:  
This helps the supermarket identify who placed each order and where the customer is located.

Result:  
Screenshot included in the screenshots folder.

 JOIN 2 – ORDER ITEMS AND PRODUCTS

Lists order items together with the product name, category, price, and quantity.
The JOIN connects order_items with products using product_id.
It allows the supermarket to see which products were purchased, their category, price and quantity in each order

Business Interpretation: 
This helps the supermarket see which products were purchased and in what quantities.

Result: 
Screenshot included in the screenshots folder.

JOIN 3 – CUSTOMERS AND ORDERS

ThE LEFT JOIN starts with the customers table, so every customer is displayed even if they have no order.

Business Interpretation:
This helps the supermarket identify both active customers and customers who have not placed an order.

Result: 
Screenshot included in the screenshots folder.

CTE QUERY

Calculates the total amount spent by each customer and identifies customers whose spending is above the average customer spending.

Business Interpretation: 
This helps the supermarket identify customers who contribute higher amounts to sales.

Result: 
Screenshot included in the screenshots folder.

WINDOW FUNCTIONS

WINDOW 1 – CUSTOMER SPENDING RANK

Ranks customers according to their total amount spent, from highest to lowest.

Business Interpretation:  
This helps the supermarket compare customer spending levels.

WINDOW 2 – ORDER NUMBERING

Numbers each customer's orders according to the order date.

Business Interpretation:  
This helps track the sequence of purchases made by each customer.

WINDOW 3 – RUNNING REVENUE TOTAL

The CTE first calculates the revenue generated on each date. 
The window function then adds each day's revenue to the previous revenue to create a running total over time.

Business Interpretation: 
This helps the supermarket monitor how total revenue increases over different dates.

WINDOW 4 – DAYS BETWEEN ORDERS

Calculates the number of days between a customer's current order and previous order.

Business Interpretation: 
This helps the supermarket understand customer purchasing frequency.

 RESULTS AND SCREENSHOTS

Screenshots of the query results are included in the `screenshots` folder.

CHALLENGES AND SOLUTIONS

One challenge was setting up and connecting to the Oracle database correctly. This was resolved by using the correct Oracle service and connection settings.

Another challenge was understanding JOINs, CTEs, and window functions. These were resolved by testing each query in Oracle SQL Developer and checking the results.

CONCLUSION

The database successfully stores and manages Sunrise Supermarket's customer, product, order, and order item information. 
The SQL queries provide useful information about customer spending, purchasing patterns, and revenue.
