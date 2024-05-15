- ### Select subquery
```mysql
select * from tableName where age > (select age from tableName where name='namita')
```
- ### Delete subquery
```mysql
delete from tableName where id=(select id from tableName where id > 20)
```
