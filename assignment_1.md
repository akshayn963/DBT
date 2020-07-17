# ASSIGNMENT 1

```
a)create table salespeople
(
  Snum int(4) PRIMARY KEY,
  Sname varchar(10) NOT NULL,
  City varchar(10) NOT NULL,
  Comm float(3,2)
);
```
```
b)create table customers
(
  Cnum int(4) PRIMARY KEY,
  Cname varchar(10) NOT NULL,
  City varchar(10) NOT NULL,
  Rating int(4),
  Snum int(4),
  FOREIGN KEY (Snum) REFERENCES salespeople (Snum)
);
```
```
c)create table orders
(
  Onum int(4) PRIMARY KEY,
  Amt float(7,2),
  Odate date,
  Snum int(4),
  Cnum int(4),
  FOREIGN KEY (Snum) REFERENCES salespeople(Snum),
  FOREIGN KEY (Cnum) REFERENCES customers (Cnum)
);
```


## insert statements for salespeople table:->>
```
1)INSERT INTO salespeople VALUES('1001', 'peel','london',.12);
2)INSERT INTO salespeople VALUES('1002', 'serres','san jose',.13);
3)INSERT INTO salespeople VALUES('1004', 'motika','london',.11);
4)INSERT INTO salespeople VALUES('1007', 'rifkin','barcelona',.15);
5)INSERT INTO salespeople VALUES('1003', 'axelrod','new york',.10);
```

## insert statements for customers table:->>

```
1)INSERT INTO customers VALUES('2001', 'hoffman','london',100,'1001');
2)INSERT INTO customers VALUES('2002', 'giovanni','rome',200,'1003');
3)INSERT INTO customers VALUES('2003', 'liu','san jose',200,'1002');
4)INSERT INTO customers VALUES('2004', 'grass','berlin',300,'1002');
5)INSERT INTO customers VALUES('2006', 'clemens','london',100,'1001');
6)INSERT INTO customers VALUES('2008', 'cisneros','san jose',300,'1007');
7)INSERT INTO customers VALUES('2007', 'pereira','rome',100,'1004');
```

## insert statements for customers table:->>

```
1)INSERT INTO orders VALUES('3001', 18.69,'90-10-03','1007','2008');
2)INSERT INTO orders VALUES('3003', 767.19,'90-10-03','1001','2001');
3)INSERT INTO orders VALUES('3002', 1900.10,'90-10-03','1004','2007');
4)INSERT INTO orders VALUES('3005', 5160.45,'90-10-03','1002','2003');
5)INSERT INTO orders VALUES('3006', 1098.16,'90-10-03','1007','2008');
6)INSERT INTO orders VALUES('3009', 1713.23,'90-10-04','1003','2002');
7)INSERT INTO orders VALUES('3007', 75.75,'90-10-04','1003','2002');
8)INSERT INTO orders VALUES('3008', 4723.00,'90-10-05','1001','2006');
9)INSERT INTO orders VALUES('3010', 1309.95,'90-10-06','1002','2004');
10)INSERT INTO orders VALUES('3011', 9891.88,'90-10-06','1001','2006');
```