- ### MAX()
- Get max value
```mysql
select max(salary) as HighSalary from tableName;
```
- ### MIN()
- Get min value
```mysql
select min(salary) as MinSalary from tableName;
```
- ### AVG()
- Get average value
```mysql
select avg(salary) as AverageSalary from tableName;
```
- ### COUNT()
- Get count value
```mysql
select count(salary) as TotalEmployee from tableName;
```
- ### Group by
- Get value group by
```mysql
select Name, max(age) as MostAge from tableName group by JobType;
```
- ### Having
- Get having value
```mysql
select Name, max(age) as MostAge from tableName group by JobType having MostAge > 30;
```
