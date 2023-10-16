# DatabaseAssignment03
# Roll-Number: 2021-CE-36

# Assignment: IT481 - Database Security and Optimization

## Unit Outcomes

- Examine Application Security concepts.
- Examine Security Layers.
- Modify the database so that tables are protected.

## Purpose

This assignment builds upon the work done in the previous unit and focuses on enhancing security and optimization in a database schema. You will implement a layered approach to develop a software application, adding user credentials, and modifying database permissions.

## Assignment Instructions

1. Create a copy of the Unit 2 application to use as a starting point for the Unit 3 application. Save this as the baseline in your chosen source code management system.
2. Add a login screen that collects server, database, username, and password for the database connection string. These values will be passed to the business layer during construction.
3. Implement access to three tables, display record counts, and create lists of data from each table.
4. Create an SQL script to prepare the database:
   - Create roles/groups for security:
     - SalesRole
     - HRRole
     - CEORole
   - Modify access for these roles/groups:
     - Grant SalesRole access to Orders and Customers tables.
     - Grant HRRole access to the Employee table.
     - Grant CEORole access to Orders, Customers, and Employee tables.
   - Create three new database users:
     - User_CEO
     - User_HR
     - User_Sales
   - Assign each user to the appropriate role/group:
     - User_Sales to SalesRole
     - User_HR to HRRole
     - User_CEO to CEORole


5. Add new methods to the business layer:
   - Create methods to return the number of employees and orders in a similar fashion as customers.
   - Include a constructor that accepts the four data items required for the connection string.
6. Modify the data layer to support the two additional tables. Note that the methods should return raw data, not a table structure.

## Reminders

- The presentation layer should only interact with the business layer.
- All interactions with the data layer must occur within the business layer.

## Assignment Requirements

1. Prepare an SQL script for the Northwind database as per the instructions and save it as `IT481_Unit3_YourName.SQL`.
2. Save your source code to a separate location, distinct from the Unit 2 project. Include a screenshot as proof and save it in a Word document named `IT481_Unit3_YourName.doc`.
3. Modify your application to require user credentials:
   - Add a GUI interface for user credentials.
   - Implement error handling.
   - Allow viewing of multiple tables.
4. Test your application using the following user accounts:
   - User_CEO should have access to all tables.
   - User_HR can only access the Employee table.
   - User_Sales can only access Customers and Orders.
   - Implement error handling for incorrect login data.

# This Code fulfills all the requirements mentioned above!
# Feel free to adapt this template to your needs, adding specific details, and customizing it for your assignment. Good luck with your IT481 - Database Security and Optimization project!
# Screenshots have been added as well to show the access of each user:

![Sales_Orders](https://github.com/SyedNoorAliDev/DatabaseAssignment03/assets/96229280/afa7d910-949c-4242-9a6c-dbab9445fd4b)
![Sales_Employees](https://github.com/SyedNoorAliDev/DatabaseAssignment03/assets/96229280/1b114844-d559-45ec-8cc0-4b68ce9f16e7)
![Sales_Cust](https://github.com/SyedNoorAliDev/DatabaseAssignment03/assets/96229280/e9ed7435-8d9f-4481-a10f-32bd8d9c1cdd)
![HR_Orders](https://github.com/SyedNoorAliDev/DatabaseAssignment03/assets/96229280/f1723365-1c6f-47b4-9dd0-22c77bbf00a0)
![HR_Emps](https://github.com/SyedNoorAliDev/DatabaseAssignment03/assets/96229280/cfc29e08-6a1f-442b-b8b2-74987022aa73)
![HR_Customers](https://github.com/SyedNoorAliDev/DatabaseAssignment03/assets/96229280/0d753c92-ce74-4979-badc-fc93dd0e38ea)
![CEO_Orders](https://github.com/SyedNoorAliDev/DatabaseAssignment03/assets/96229280/b719f060-97f5-429d-be86-943d69d77ca7)
![CEO_Emps](https://github.com/SyedNoorAliDev/DatabaseAssignment03/assets/96229280/861038f8-b6ab-443b-bbae-a429b9862fd8)
![CEO_Cust](https://github.com/SyedNoorAliDev/DatabaseAssignment03/assets/96229280/47082673-53ff-4e3f-a991-2153da255e6c)

