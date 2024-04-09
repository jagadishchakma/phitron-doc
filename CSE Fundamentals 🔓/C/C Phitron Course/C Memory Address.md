# Introduction
- When a vairable is created in C, a memory address is assigned to the variable.
- The memory address is the location of where the variable is stored on the computer.
- When we assign a value to the variable, it is stored in this memory address.
- To access it, use the reference operator ==&== , and the result represents where the variable is stored.
- To see memory address use the ==%p== format-specifier.
- To store memory address in a variable use pointer * .

# Usese Keywords
- & = The Empersand
- %p = format specifier
- * = The Asterisk

###### syntax
```c
int a; // created a memory address for this variable
a = 10; // assign 10 value to this memeory address space
printf("%p", &a) // see memory address name
int* b = &a // store memory address
```


# Access Memory Address
```c
int a; // create memory address for a
&a // access memory address
```

# Store Memory Address
```c
int a; // create memory address
int* b = &a; // store memory address
```


# Print Memory Address
```c
int a; // create memory address
int* b = &a; // store memory address
printf("%p",b); // print memroy address
printf("%p", &a); // print memory address
```


# Print Store Memory Address Value
```c
int a; // created a memory address for a
a=230; // assign  value to created memroy address
int* b = &a; // store memory address
printf("%d",*b); // print store memory address value
```


# Assign Value To Store Memory Address 
```c
int a; // created memroy address for a
int* b = &a; // store memroy address for b
*b = 230; // assign value for store memory address
```

**Note: store memory address is called also ==pointer.==**


# Why is it usefull to know the memory address?
- Pointers are important in C, because they allow us to manipulate the data in the computer's memory - **this can reduce the code and improve the performance.**
- Pointers are one of the things that make C stand out from other programming languages, like Python and Java.
