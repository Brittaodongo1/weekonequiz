-- answers.sql

--  Retrieve the checkNumber, paymentDate, and amount from the payments table
SELECT checkNumber, paymentDate, amount
FROM payments;

--  Retrieve the orderDate, requiredDate, and status of orders that are 'In Process'
-- Sort in descending order of orderDate
SELECT orderDate, requiredDate, status
FROM orders
WHERE status = 'In Process'
ORDER BY orderDate DESC;

--  Display the firstName, lastName, and email of employees whose job title is 'Sales Rep'
-- Order in descending order of employeeNumber
SELECT firstName, lastName, email
FROM employees
WHERE jobTitle = 'Sales Rep'
ORDER BY employeeNumber DESC;

--  Retrieve all columns and records from the offices table
SELECT *
FROM offices;

--  Fetch productName and quantityInStock from the products table
-- Sort in ascending order of buyPrice and limit to 5 records
SELECT productName, quantityInStock
FROM products
ORDER BY buyPrice ASC
LIMIT 5;
