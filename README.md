# First Data Analysis Project

## Overview

This project involves the analysis of a company database that contains information about employees, branches, clients, and suppliers. The database is structured to facilitate various data operations and analyses, such as sales performance, employee management, and client interactions.

## Database Structure

The database is named `CompanyDatabase` and consists of the following tables:

### Tables

1. **Employee**
   - `emp_id`: INT, Primary Key
   - `first_name`: VARCHAR(40)
   - `last_name`: VARCHAR(40)
   - `birth_day`: DATE
   - `sex`: VARCHAR(1)
   - `salary`: INT
   - `super_id`: INT (Supervisor ID)
   - `branch_id`: INT (Foreign Key)

2. **Branch**
   - `branch_id`: INT, Primary Key
   - `branch_name`: VARCHAR(40)
   - `mgr_id`: INT (Manager ID)
   - `mgr_start_date`: DATE

3. **Client**
   - `client_id`: INT, Primary Key
   - `client_name`: VARCHAR(40)
   - `branch_id`: INT (Foreign Key)

4. **Works With**
   - `emp_id`: INT (Foreign Key)
   - `client_id`: INT (Foreign Key)
   - `total_sales`: INT
   - Primary Key: (`emp_id`, `client_id`)

5. **Branch Supplier**
   - `branch_id`: INT (Foreign Key)
   - `supplier_name`: VARCHAR(40)
   - `supply_type`: VARCHAR(40)
   - Primary Key: (`branch_id`, `supplier_name`)

## Data Insertion

The database is populated with sample data, which includes:

- Employees from different branches (Corporate, Scranton, Stamford)
- Branches and their respective managers
- Clients associated with branches
- Suppliers providing materials to branches
- Sales records indicating which employees worked with which clients and the corresponding sales amounts.

## Setup

To set up the database:

1. Run the SQL commands to create the database and tables.
2. Insert the sample data as provided in the SQL scripts.

## Usage

You can perform various SQL queries to analyze employee performance, branch sales, and client interactions. For example:

- Retrieve total sales by each employee.
- Find out which clients are serviced by each branch.
- Analyze the salary distribution across different branches.

## Dashboard

![Company Database Dashboard](https://github.com/Morobang/First-Data-Analysis-Project/blob/main/Company%20Database%20Dashboard.png)

## Conclusion

This project serves as a foundational example of using SQL databases for business analysis. You can extend it further by adding more features, such as reporting tools or user interfaces.

## License

This project is licensed under the MIT License.


 
