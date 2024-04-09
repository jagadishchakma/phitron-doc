# Phitron
- C ==if__else== vs C++ ==if__else== are same.
- C, C++ both have ternary operator or if..else shorthand.
```c++
string result = (12 > 4) ? "Greater than": "less than";
cout << result;
```

# If Else
C++ has the following conditional statements:
- Use ==if== to specify a block of code to be executed, if a specified condition is true.
- Use ==else== to specify a block of code to be executed, if the same condition is false.
- Use ==else if== to specify a new condition to test, if the first conditin is false.

##### Type One
```c++
if(condition){
	// code will be executed if condition is true
}
```

##### Type Two
```c++
if(condition){
	// cond will be executed if condition is true.
}else{
	// code will be executed if condition is false.
}
```

##### Type Three
```c++
if(condition){
	// code will be executed if condition is true.
}else if(condition){
	// code will be executed if before conditon is false and it's true
}else{
	// code will be executed if all condition is false.
}
```

#### Notices
==else fi()== condition you can define many times.

----

# Ternary Operator (Short Hand If Else)
There is also a short-hand if else, which is known as the ==ternary operator== because it consists of three operands.

```c++
string result = (10 > 5) ? "Greather thant 5": "Less than 5";
cout << result;
```
