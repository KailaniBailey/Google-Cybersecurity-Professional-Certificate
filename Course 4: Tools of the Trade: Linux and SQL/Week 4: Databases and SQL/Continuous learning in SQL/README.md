# Continuous learning in SQL
You've explored a lot about SQL, including applying filters to SQL queries and joining multiple tables together in a query.  There's still more that you can do with SQL. This reading will explore an example of something new you can add to your SQL toolbox: aggregate functions. You'll then focus on how you can continue learning about this and other SQL topics on your own.

## Aggregate functions
In SQL, **aggregate functions** are functions that perform a calculation over multiple data points and return the result of the calculation. The actual data is not returned. 

There are various aggregate functions that perform different calculations:

- COUNT returns a single number that represents the number of rows returned from your query.
- AVG returns a single number that represents the average of the numerical data in a column.
- SUM returns a single number that represents the sum of the numerical data in a column. 

### Aggregate function syntax
To use an aggregate function, place the keyword for it after the SELECT keyword, and then in parentheses, indicate the column you want to perform the calculation on.

For example, when working with the customers table, you can use aggregate functions to summarize important information about the table. If you want to find out how many customers there are in total, you can use the COUNT function on any column, and SQL will return the total number of records, excluding NULL values. You can run this query and explore its output:

[ Text only ]

1. SELECT COUNT(firstname)
2. FROM customers;

[ Insert photo of output. ]

The result is a table with one column titled COUNT(firstname) and one row that indicates the count. 

If you want to find the number of customers from a specific country, you can add a filter to your query:

[ Text only ]

1. SELECT COUNT(firstname)
2. FROM customers
3. WHERE country = 'USA';

[ Insert photo of output. ]

With this filter, the count is lower because it only includes the records where the country column contains a value of 'USA'.

There are a lot of other aggregate functions in SQL. The syntax of placing them after SELECT is exactly the same as the COUNT function.

## Continuing to learn SQL
SQL is a widely used querying language, with many more keywords and applications. You can continue to learn more about aggregate functions and other aspects of using SQL on your own.

Most importantly, approach new tasks with curiosity and a willingness to find new ways to apply SQL to your work as a security analyst. Identify the data results that you need and try to use SQL to obtain these results.

Fortunately, SQL is one of the most important tools for working with databases and analyzing data, so you'll find a lot of support in trying to learn SQL online. First, try searching for the concepts you've already learned and practiced to find resources that have accurate easy-to-follow explanations. When you identify these resources, you can use them to extend your knowledge.

Continuing your practical experience with SQL is also important. You can also search for new databases that allow you to perform SQL queries using what you've learned.

## Key takeaways
Aggregate functions like COUNT, SUM, and AVG allow you to work with SQL in new ways. There are many other additional aspects of SQL that could be useful to you as an analyst. By continuing to explore SQL on your own, you can expand the ways you can apply SQL in a cybersecurity context.
