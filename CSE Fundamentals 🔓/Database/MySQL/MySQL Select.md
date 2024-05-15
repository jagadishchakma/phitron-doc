- ### Select All
```mysql
select * from tableName;
```
- ### Select Specific Field
```mysql
select Name, Age, Roll, City from tableName;
```
- ### Select Using "Where"
```mysql
select * from tableName where roll = 123 and age = 23
```
- ### Select Using Arithmetic Operator
```mysql
select salary+extra from tableName
```
- ### Select Using Comparison Operator
```mysql
select * from tableName where age > 18
```
- ### Select Using Logical Operator
```mysql 
select * from tableName where age > 18 or married == "YES"
```
- ### Select Using "Distinct" Unique record
```mysql
select distinct * from tableName;
```
- ### Select Using "Order By" 
```mysql
select * from tableName order by desc;
```
- ### Select Using "limit offset."
```mysql
select * from tableName limit 10 offset 30;
```
- ### Select Using "like %%"
```mysql
select * from tableName where name like '%chakma%'
select * from tableName where name like 'chakma%'
select * from tableName where name like '%chakma'
```
- ### Select Using As
```mysql
select FullName as Name, Age, City from tableName
```
