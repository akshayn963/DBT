# Assignment 4

```
   Q1) Write a select command that produces the order number, amount, and date for all rows in the Orders table.
   ans--> select Onum,Amt,Odate from orders;
```
```
   Q2)Write a query that produces all rows from the Customers table for which the salesperson’s number is 1001.
   ans--> select * from customers where Snum='1001';
```
```
   Q3) Write a query that displays the Salespeople table with the columns in the following order: city, sname, snum, comm.
   ans--> select City,Sname,Snum,Comm from salespeople;
```
```
   Q4)Write a select command that produces the rating followed by the name of each customer in San Jose.
   ans-->select rating,cname from customers where City='san jose';
```
```
   Q5)Write a query that will produce the snum values of all salespeople (suppress the duplicates) with orders in the Orders table.
   ans--> select distinct snum from orders;
```   