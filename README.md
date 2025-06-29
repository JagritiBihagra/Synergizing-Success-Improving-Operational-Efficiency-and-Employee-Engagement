# Synergizing-Success-Improving-Operational-Efficiency-and-Employee-Engagement

This project is part of a SQL capstone focused on addressing key operational inefficiencies and employee engagement strategies within a multi-departmental business. It utilizes SQL queries and database objects to extract insights related to employee performance, product sales, inventory, and more.

## Problem Statement
Problem Statement:
Enhancing Operational Efficiency and Growth Strategies in a Multi-Departmental
Business
Context:
● Business operations involve a complex interaction between departments,
products, suppliers, and employees, where each element contributes to
overall performance. Challenges such as managing inventory levels,
optimizing employee performance, maintaining customer satisfaction, and
navigating supply chain dependencies require constant data analysis for
informed decision-making. Effective alignment between leadership,
employees, and market trends is also crucial for future planning and
sustainable growth. 
Problem:
● The company is experiencing several operational inefficiencies:
● Employee Performance & Retention Challenges: Inconsistent employee
performance and high turnover rates negatively impact productivity. The
company needs to evaluate whether training programs, salary, and tenure
influence employee retention and performance.
● Product Sales & Customer Satisfaction Issues: Some products have low
customer feedback scores despite high sales, indicating potential quality or
support issues. Additionally, low sales for certain products may suggest
gaps in marketing strategies or misalignment with market demands.
● Supply Chain & Inventory Management Issues: Supply chain risks are
posed by low inventory levels approaching reorder points, potentially
leading to missed sales opportunities if not addressed promptly.
● Technology Usage & Future Planning Concerns: The company is
underutilizing technology in several departments, leading to inefficiencies.
Weak market research and unclear company direction could affect
long-term growth and competitiveness.


This project aims to analyze operational data to identify patterns and recommend solutions using structured SQL queries.

## Project Files

| File Name         | Description                                                  |
|------------------|--------------------------------------------------------------|
| `SynSuccess.sql`  | SQL script containing all queries, views, indexes, procedures, and triggers |
| `README.md`       | Documentation describing the project and its components      |

## Analysis Objectives

### Employee Performance
- Identify the department with the highest average profit margin.
- Find the top-performing employee in the IT department and their role.

### Product Sales and Customer Satisfaction
- Determine the highest revenue-generating product in the HR department.
- Calculate the average customer feedback score in the Accessories category and identify the highest-rated product.

### Supply Chain and Inventory
- Identify the supplier with the highest total inventory across departments.
- Find the product with the lowest inventory level in the Gadgets category.

### Employee Training and Sales
- Count the number of Sales department employees who completed training.
- Calculate what percentage of Sales employees have completed training.

### Product Sales Contribution
- Calculate the total units sold for Marketing department products.
- Determine the product that contributed the most to that total.

## Advanced SQL Features

This project includes implementations of the following advanced SQL constructs:

- **Window Functions**: Rank employees by revenue within each department.
- **Common Table Expressions (CTEs)**: Compute average salaries and filter departments with averages above $70,000.
- **Views**: A view for Accessories products showing product name, revenue, and profit margin.
- **Indexes**:
  - Non-clustered index on the `employee_name` column.
  - Clustered index on the `company_id` column.
- **Stored Procedure**: Returns total revenue by department using a parameter.
- **Trigger**: Logs changes to the `revenue` column into a separate audit table.
- **Scalar User-Defined Function (UDF)**: Calculates profit from revenue and profit margin.

## Requirements

- SQL Server (T-SQL)
- A table named `Business_Operations_Dataset$` with relevant fields, including:
  - `employee_id`, `employee_name`, `department`, `salary`, `training_program_completed`, `employee_performance_score`, `revenue`, `units_sold`, `inventory_level`, `customer_feedback_score`, `supplier_id`, `supplier_name`, `product_name`, `product_id`, `category`, `profit_margin`, `company_id`, `role`

## How to Use

1. Set up a SQL Server database and create a table named `Business_Operations_Dataset$` with sample or provided data.
2. Run the `SynSuccess.sql` script to execute all queries and create views, indexes, procedures, triggers, and functions.
3. Use the outputs to perform analysis, build dashboards, or generate reports.


## License

© Intellipaat. All rights reserved. This project is intended for educational use only.
