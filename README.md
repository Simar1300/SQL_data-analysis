
# Finance Analytics SQL Project

## Overview
This project focuses on analyzing sales and financial data from a retail database. The database consists of various tables that store information about customers, products, sales transactions, and costs. The main objective is to derive insights related to sales performance, customer behavior, and financial metrics, particularly for the customer "Croma" in India.

## Database Structure
The database is organized into the following tables:
- **dim_customer**: Contains customer details, including customer codes and market information.
- **dim_product**: Stores product information, including product codes, names, and variants.
- **dimdate**: Holds date-related data to facilitate time-based analyses.
- **fact_sales_monthly**: Records monthly sales transactions, including quantities sold and associated customer codes.
- **fact_gross_price**: Contains gross pricing information for products, associated with different fiscal years.
- **fact_forecast_monthly**, **fact_freight_cost**, **fact_manufacturing_cost**, **fact_post_invoice_deductions**, and **fact_pre_invoice_deductions**: Additional tables for various financial metrics and costs related to the products and sales.

## Key Features

### 1. Customer and Sales Analysis
- **Customer Segmentation**: Extract specific customer codes (e.g., Croma India) for targeted analysis.
- **Sales Trends**: Analyze monthly sales performance across fiscal years to identify patterns and fluctuations. 
- **Product-Based Insights**: Track product-wise sales to identify top-performing products and their contribution to revenue.

### 2. Gross Sales and Financial Reporting
- **Gross Sales Calculation**: Calculate monthly gross sales by combining sales quantity with product prices from the **fact_gross_price** table. 
- **Market-Level Financial Status**: Evaluate market performance (e.g., India) and assign badges ("Gold" or "Silver") based on the total sales volume for a fiscal year.

### 3. SQL Functions and Stored Procedures
- **Fiscal Year Calculation**: Implemented a **user-defined SQL function** to accurately calculate fiscal years, which helps align business reporting timelines.
- **Monthly Sales Reporting Procedure**: Developed a **stored procedure** to generate monthly sales reports dynamically for any customer using input parameters.
- **Market Badge Assignment Procedure**: A **stored procedure** that determines the market’s performance status (Gold/Silver) based on total sales quantity.
  
## Performance Insights
This project aims to provide actionable insights into the sales and financial health of the business. By utilizing advanced SQL queries, functions, and procedures, users can:  
- Identify trends and seasonal effects on sales.
- Track key customers and their performance over time.
- Understand which products or product variants contribute most to revenue.
- Assess market performance to guide strategic decisions (e.g., Gold/Silver badges for market status).


## Future Enhancements
Future improvements that can be implemented include:
- **Predictive Analytics**: Adding forecasting models to predict future sales trends.
- **Visualization Dashboards**: Using Power BI, Tableau, or similar tools to create interactive dashboards for better data visualization.
- **Incorporating Additional Metrics**: Extending the analysis to include shipping costs, manufacturing costs, and pre- and post-invoice deductions for a more comprehensive view of profitability.



## Installation and Usage
1. **Database Setup**: Ensure you have access to a SQL database and the necessary permissions to create functions and procedures.
2. **Import Tables**: Load the provided data tables into your SQL environment.
3. **Run Queries and Procedures**: Use the SQL scripts provided in the project to execute functions, queries, and stored procedures for generating reports.


## Contribution
Contributions are welcome! If you have suggestions for improvements or additional features, feel free to open an issue or submit a pull request.

## Acknowledgments
- Special thanks to the contributors and maintainers of SQL databases and analytical techniques that made this project possible.
- Inspired by real-world retail analytics scenarios.

