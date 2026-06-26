# Zepto-SQL-Data-Analyst-Portfolio

Project Overview
This project demonstrates SQL-based data exploration, cleaning, and business analysis on a Zepto grocery inventory dataset. The goal is to analyze product information, perform data cleaning, and generate actionable business insights using SQL queries.

The project covers the complete workflow from creating the database table to answering real-world business questions.

Project Workflow

1. Database Creation
- Created the zepto table
- Defined appropriate data types
- Assigned sku_id as the primary key

2. Data Exploration
Performed initial analysis to understand the dataset:
  - Count total number of rows
  - View sample records
  - Identify NULL values
  - List unique product categories
  - Compare products that are in stock vs out of stock
  - Identify duplicate product names

3. Data Cleaning
Data preprocessing included:
  - Identifying products with zero prices
  - Removing invalid records (MRP = 0)  
  - Converting prices from paise (cents) to rupees by dividing by 100

Business Insight Queries
The following business questions were answered using SQL:

1. Top 10 Best Value Products
Identified products offering the highest discount percentages.

2. High MRP Products Currently Out of Stock
Retrieved expensive products that are unavailable.

3. Estimated Revenue by Category
Calculated potential revenue using:
Revenue = Discounted Selling Price × Available Quantity

4. Premium Products with Low Discounts
Found products with:
MRP greater than ₹500
Discount less than 10%

5. Categories with Highest Average Discounts
Ranked categories based on average discount percentages.

6. Best Value by Price per Gram
Calculated:
Price per Gram = Discounted Selling Price ÷ Weight
Filtered products weighing at least 100 grams.

7. Product Weight Classification
Grouped products into:
Low (<1000g)
Medium (1000g–4999g)
Bulk (5000g and above)
using SQL CASE statements.

8. Total Inventory Weight per Category
Calculated the total inventory weight available in each category.

Project Structure
Zepto-SQL-Analysis/
│
├── Zepto SQL Codes.sql          # SQL script containing all queries
├── README.md                    # Project documentation
└── zepto_v2.csv                 # Dataset 

Learning Outcomes
Through this project, I practiced:
  - Database design
  - Data exploration
  - Data cleaning using SQL
  - Writing analytical SQL queries
  - Solving business problems with SQL
  - Using aggregate functions and conditional logic
  - Working with real-world retail inventory data

Future Improvements
Possible enhancements include:
  - Creating SQL views for reporting
  - Building stored procedures
  - Adding indexes for query optimization
  - Developing an interactive dashboard using Power BI or Tableau
  - Performing time-series sales analysis if transactional data becomes available
