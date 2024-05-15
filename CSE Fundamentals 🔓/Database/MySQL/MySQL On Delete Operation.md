- ### Primary key record delete than her foreign key delete
```mysql
foreign key(S_Roll) references Student(Roll) on delete cascade;
foreign key(S_Roll) references Student(Roll) on delete set null;
```
