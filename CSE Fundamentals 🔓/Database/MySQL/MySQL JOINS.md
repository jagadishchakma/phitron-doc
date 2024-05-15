- ### Join manually
```mysql
select table1.*, table2.* from table1,table2 where table1.id = table2.id;
select * from table1,table2 where table1.id = table2.id;
```

- ### Join using keyword
```mysql
select table1.*, table2.* from tabl1 join table2 on table1.id = table2.id;
select * from table1 join table2 on table1.id = table2.id;
select * from table1 join table2 using(id); ###if field_name same
```
- ### Join using inner,left,right,cross join
```mysql
select * from table1 left join table2 using(id);
select * from table1 right join table2 using(id
select * from table1 inner join table2 using(id);
select * from table1 cross join table2 using(id);
```

- ### Self join
```mysql
select * from table1 as one1 join table1 as two2 where one1.id = two2.roll
```
