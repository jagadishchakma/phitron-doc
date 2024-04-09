# Introdcution
Arrays are used to store multiple values in  a single variable, instead of declaring separate variables for each value.

# Array With Memory
- Array sequentially store in memory followed by the first index and space data type.

###### Single Variable 10 Values
```c
int a, b, c, d, e, f, g, h, i, j;
a = 1;
b = 2;
c = 3;
d = 4;
e = 5;
f = 6;
g = 7;
h = 8;
i = 9;
j = 10;
```
###### ==Single Variable In Memory==
|4|4|4|4|4|4|4|4|4|4|
|:--|:--|:--|:--|:--|:--|:--|:--|:--|:--|
##### Array With 10 Values
```c
int a[10] = {1,2,3,4,5,6,7,8,9,10};
```
###### ==Array Variable In Memory==
|int|int|int|int|int|int|int|int|int|int|
|:--|:--|:--|:--|:--|:--|:--|:--|:--|:--|


# Why We Need Array?
- For storing multiple values in a signle variable.
- For data manipulation in easy to way.
- For data shorting.

# Create An Array

##### Array Initialization
```c
data_type array_name[] = {value};
```

##### Array Declare
```c
data_type array_name[size];
```


##### Examples
```c
int a[]  = {1,2,3,4,5};
int a[5];
```

# Access In Array ==!important==
```c
array[index];
```
- Array index start from zero 0.
###### How to work behind the scene?
- array_name assign first index address by default.
- then sequentilay access using index * data_size.
###### Example
```c
int a[4] = {560,56,789,4};
a[0];
a[1];
a[...];
```

|int|int|int|int|
|:--|:--|:--|:--|
|0|1|2|3|
|a+a[0*size]|a+a[1*size]|a+a[2*size]|a+a[3*size]|

