# SQL Notes

RDBMS stands for Relational Database Management System.
The data in RDBMS is stored in database objects called tables. A table is a collection of related data entries and it consists of columns and rows.

```html
SELECT DISTINCT Country FROM Customers;       Select all the different values from the Country column in the Customers table.

SELECT * FROM Customers
WHERE Country='Germany' AND (City='Berlin' OR City='München');         Select all records where the Country column has the value "Germany" and city is berlin or münchen

INSERT INTO Customers (CustomerName, City, Country)
VALUES ('Cardinal', 'Stavanger', 'Norway');                            Insert a new record 

UPDATE Customers
SET ContactName = 'Alfred Schmidt', City= 'Frankfurt'                  Updates the first customer (CustomerID = 1) with a new contact person and a new city.
WHERE CustomerID = 1;

DELETE FROM Customers WHERE CustomerName='Alfreds Futterkiste';        Deletes the customer "Alfreds Futterkiste" from the "Customers" table

SELECT COUNT(ProductID)                              Finds the number of products
FROM Products;

SELECT SUM(Quantity)                                 Sum of the "Quantity" fields in the "OrderDetails" table
FROM OrderDetails;

SELECT * FROM Customers                              Selects all customers with a CustomerName starting with "a"
WHERE CustomerName LIKE 'a%';

SELECT * FROM Customers                              Selects all customers that are NOT located in "Germany", "France" or "UK"
WHERE Country NOT IN ('Germany', 'France', 'UK'); 

SELECT CustomerName AS Customer, ContactName AS [Contact Person]      Creates two aliases, one for the CustomerName column and one for the ContactName column.
FROM Customers;

SELECT Orders.OrderID, Customers.CustomerName, Orders.OrderDate          "CustomerID" column in the "Orders" table refers to the "CustomerID" in the "Customers" table.
FROM Orders                                                               The relationship between the two tables above is the "CustomerID" column.
INNER JOIN Customers ON Orders.CustomerID=Customers.CustomerID;

SELECT Shippers.ShipperName, COUNT(Orders.OrderID) AS NumberOfOrders FROM Orders
LEFT JOIN Shippers ON Orders.ShipperID = Shippers.ShipperID                          Lists the number of orders sent by each shipper
GROUP BY ShipperName;

SELECT * INTO CustomersBackup2017 IN 'Backup.mdb'                          IN clause to copy the table into a new table in another database
FROM Customers;  

```












