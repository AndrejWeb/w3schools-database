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
    
    
 A SQL Join statement is used to combine data or rows from two or more tables based on a common field between them. Different types of Joins are:

INNER JOIN
LEFT JOIN
RIGHT JOIN
FULL JOIN
Consider the two tables below:

Student

Screenshot from 2016-12-19 12-53-29

StudentCourse




table5

 

The simplest Join is INNER JOIN.

INNER JOIN: The INNER JOIN keyword selects all rows from both the tables as long as the condition satisfies. This keyword will create the result-set by combining all rows from both the tables where the condition satisfies i.e value of the common field will be same.
Syntax:
SELECT table1.column1,table1.column2,table2.column1,....
FROM table1 
INNER JOIN table2
ON table1.matching_column = table2.matching_column;


table1: First table.
table2: Second table
matching_column: Column common to both the tables.
Note: We can also write JOIN instead of INNER JOIN. JOIN is same as INNER JOIN.

Click to enlarge

Example Queries(INNER JOIN)

This query will show the names and age of students enrolled in different courses.
SELECT StudentCourse.COURSE_ID, Student.NAME, Student.AGE FROM Student
INNER JOIN StudentCourse
ON Student.ROLL_NO = StudentCourse.ROLL_NO;
Output:
table2

LEFT JOIN: This join returns all the rows of the table on the left side of the join and matching rows for the table on the right side of join. The rows for which there is no matching row on right side, the result-set will contain null. LEFT JOIN is also known as LEFT OUTER JOIN.Syntax:
SELECT table1.column1,table1.column2,table2.column1,....
FROM table1 
LEFT JOIN table2
ON table1.matching_column = table2.matching_column;

   
