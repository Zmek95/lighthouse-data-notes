# Lecture Notes Week 2 Day 1

SQL is a declaritive programming language. Writing order does not determine order of operations!

Good tutorial on order of operations: https://learnsql.com/blog/sql-order-of-operations/

## General guildline for SQL query order of operation:
![SQL_query_order](sql_order.png "SQL query order")
Note: The order may change depending on which clauses are present in the query.

#### Answers to questions in lecture:
SELECT bar, type, price FROM menu_items
JOIN drinks ON menu_items.drink_id = drinks.drink_id
WHERE price = (SELECT MIN(price) FROM menu_items); 

SELECT SUM(quantity), type, bar FROM orders
JOIN drinks ON orders.drink_id = drinks.drink_id
WHERE type LIKE '%beer%'
GROUP BY bar
ORDER BY SUM(quantity) DESC;
