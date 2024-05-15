- ### PRIMARY KEY
- ### FOREIGN KEY
- ### UNIQUE
- ### CHECK
- ### DEFAULT
- ### NOT NULL
```mysql
create table Student
(
	Name varchar(50) not null,
	Roll int primary key,
	email varchar(200) unique not null,
	phone int,
	age int check(age > 18)
);

create table Class11
(
	Id int primary key,
	S_Roll int unique not null,
	start datetime,
	end datetime,
	foreign key (S_Roll) references Student(Roll)
)
```
