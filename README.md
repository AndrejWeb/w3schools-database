# W3Schools Database

I'm not associated with W3Schools but I have to give them a big shout-out. This is their website:
https://www.w3schools.com

They provide excellent tutorials on the topic of web development. More than 15 years ago in the early 2000s when I was barely a teenager, I discovered their site and that's when I became interested in web development and started learning things little by little.

Anyway this repository contains the database they use for their SQL tutorial here:
https://www.w3schools.com/sql/default.asp

You can see the database tables and the data on the right hand side if you run this example:
https://www.w3schools.com/sql/trysql.asp?filename=trysql_select_all

However, there is nowhere a link to download the database so I decided to create a SQL code for it which I hope you'll find useful because it is nice to have this database locally where you can perform all sorts of SQL queries, tests, for practicing and learning purposes etc. Enjoy!

When the SQL file is executed it creates database named __w3schools__ with the following tables

    categories
    customers
    employees
    orders
    order_details
    products
    shippers
    suppliers
    
and inserts the respective data. 

You can change the database name if you want by modifying these 2 lines of code

    CREATE DATABASE IF NOT EXISTS `w3schools`
    USE `w3schools`;
