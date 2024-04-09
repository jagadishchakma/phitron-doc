# Introduction
- A **pointer** is a variable that stores the memory address of another variable as its value.
- A pointer variable points to data type of the same type, and is created with the * operator.
###### syntax
```c
int a;
int* b = &a // this variable is called pointer;
```


# Dereference
- You can also get the value of the variable the poiner points to, by using the * operator (the **Dereference** operator).
```c
int a = 10;
int* b = &a; // reference operator and its hold expression is called pointer
int c = *b; // dereference operator 
printf("%d", c);
```

# Note That
Note that the * sign can be confusing here, as it does two different things in our code:
 - When used in declaration ==(int* a)== , it creates a ==pointer variable==.
 - When not used in declaration, it act as a ==dereference operator==.


# Notes On Pointer
Pointers are one of the things that make C stand out from other programming languages, like Python and Java.
They are important in C, because they allow us to manipulate the data in the computer's memory . This can reduce the code and improve the performance. If you are familiar with data structures like lists, trees and graphs, you should know that pointers are specially useful for implementing those. And sometimes you even have to use pointer.

But be careful; pointers must be handled with care, since it is possible to damage data stored in other memory address.
