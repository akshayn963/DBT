# EXERCISE 1

```
1)create table SEMP
(
EMPNO char(4),
EMPNAME char(20),
BASIC float(9,2),
DEPTNO char(2),
DEPTHEAD char(4)
);
```
```
2)create table SDEPT
(
DEPTNO char(2),
DEPTNAME char(15)
);
```
```
3)
   a)insert into SDEPT values('10','Devlopment');

   b)insert into SDEPT values('20','Training');
```
```
4) 
   a)insert into SEMP values('0001','SUNIL',6000,'10','NULL');

   b)insert into SEMP values('0002','HIREN',8000,'20','NULL');

   c)insert into SEMP values('0003','ALI',4000,'10','0001');

   d)insert into SEMP values('0004','GEORGE',6000,NULL,'0001');
```   
```
--->create table s
        (
         `s#`char(4),
         Sname varchar(10),
         status char(10),
         city varchar(10)
        );
```

```
--->   create table p
        (
         `p#` char(4),
          Pname varchar(10),
          color varchar(10),
          weight float(7,2),
          city varchar(10)
        );
```
```
 --->     create table j
       (
        `j#` char(4),
         jname varchar(10),
         city varchar(10)
       );
```
```
 --->      create table spj
       ( 
        `s#` char(4),
        `p#` char(4),
        `j#` char(4),
        qty float(7,2)
       ); 
```
```
----> insert into s values('s1','jack','10','london'),
                          ('s2','seer','30','LA'),
                          ('s3','ryan','20','bombay'),
                          ('s4','alex','50','budapest'),
                          ('s5','max','40','paris'),
                          ('s6','stuart','70','athens');
```
```
---->insert into p values ('p1','a','red',13,'bombay'),
                          ('p2','b','black',20,'LA'),
                          ('p4','d','blue',10,'london'),
                          ('p5','f','silver',17,'paris'),
                          ('p3','c','green',19,'london');
```
```
---->insert into j values ('j1','q','paris'),
                          ('j2','s','LA'),
                          ('j4','u','bombay'),
                          ('j5','w','LA'),
                          ('j3','t','athens');
```
```
---->insert into  spj values ('s1','p2','j1','2'),
                             ('s2','p3','j5','6'),
                             ('s3','p1','j2','3'),
                             ('s6','p5','j4','8'),
                             ('s4','p2','j3','10');
```
```
5) select * from s;
```
```
6)select `s#`,sname from s;
```
```
7) select pname,color from p where CITY='London';
```
```
8) select * from s where CITY='London';
```
```
9) select * from s where CITY='Paris' or CITY='Athens';
```
```
10) select * from j where CITY='Athens';
```
```
11) select Pname,weight from p where weight between 12 and 14;
```
```
12) select * from s where status>=20;
```
```
13) select * from s where city!='London';
```
```
14) select city from s;
```
```
15)
   a) select weight*1000 from p; --->milligrams
   b)select weight/1000 from p; ---> kilograms
```