

--- start-multi-column: ID_v7nw
```column-settings
Number of Columns: 2
Largest Column: standard
```

# <p align="center">python string</p>

---
### ==string== is object this have own properties and methods.
```python
print(dir("Hello"))
```

---
### Declare
```python
str = "string" # string declare using double quotation
str = 'string' # string declare using single quotation
str = f"string" # formatted string literals
```

---
### Quotes Inside Quotes
- You can use quotes inside a string, as long as they don't match the quotes surrounding the string.
```javascript
str = "It's time to learning string";
str = 'Her name is "String"';
```

---
### Formatted Strings
- Formatted are strings use f"".
- Inside formatted strings can possible execute python code using {}.
```python
fname = "Jagadish"
lname = "Chakma"
fullName = f"Fullname is {fname} {lname}"
```

---
### Escape Characters
```python
\' insert signle quote
\" insert double quote
\\ insert backslash
\n insert a new line
\t insert new tab
\b insert a backsapce
```

---
### Multi Line Strings
- You can assign a multiple string to a variable by using the three single or double quotes.
```python
para = """
line one
line two
line three
line four
"""
print(para);
```

---
### Strings are Arrays
- Strings as like array so can do perform looping, accessing like arrays.
```python
str = "Hello World"
print((str[1])
for lett in str:
	print(lett)

```

---
### String Length
```python
str = "Hello World"
print(len(str))
```

---
### Check String
```python
str = "Hello World Python"
print("Python" in str) # check one
print("JavaScript" not in str) # check two

if "Python" in str: #check one
	pass;

if "JavaScript" not in str: #check two
	pass;

```

---
### Slicing String
```python
str = "Hello Python World String"

print(str[2:5]) #slice position to position

print(str[:5]) #slice start to position

print(str[5:]) #slice position to end

print(str[:]) #slice start to end

print(str[-1:-6:-1]) #slice end to position

print(str[-1::-1]) # slice end to start
```

---
### Upper Case
```python
str = "Hello Python World"
print(str.upper())
```

---
### Lower Case
```python
str = "Hello Python World"
print(str.lower())
```

---
### Remove Whitespace
```python
str = "              Hello Python World                    "
print(str.strip())
```

---
### Replace String
```python
str = "Hello Python World"
print(str.replace("world","Programmer"))
```

---
### Split String
```python
str = "Hello Python World"
print(str.split(" "))
```

---
### String Concatenate 
```python
str1 = "Hello"
str2 = "World"
print(str1 + " " + str2)
```


--- column-break ---

# <p align="center">javascript string</p>

---
### ==string== is object this have own properties and methods.
```python
console.dir(new String("Hello"))
```

---
### Declare
```javascript
let str = "string"; // string declare using double quotation
let str = 'string'; // string declare using single quotation
let str = `string`; // template string literals
```

---
### Quotes Inside Quotes
- You can use quotes inside a string, as long as they don't match the quotes surrounding the string.
```javascript
let str = "It's time to learning string";
let str = 'Her name is "String"';
```

---
### Template Strings
- Templates are strings enclosed in backticks (`This is a template string`).
- Inside template strings can possible execute Javascript code using ${}.
```javascript
let fname = "Jagadish";
let lname = "Chakma";
let fullName = `Fullname is ${fname} ${lname}`;
```

---
### Escape Characters
```javascript
\' insert signle quote
\" insert double quote
\\ insert backslash
\n insert a new line
\t insert new tab
\b insert a backsapce
```

---
### Multi Line Strings
- You can assign a multiple string to a variable by using the template literals.
```javascript
let para = `
line one
line two
line three
line four
`;
console.log(para);
```

---
### Strings are Arrays
- Strings as like array so can do perform looping, accessing like arrays.
```javascript
let str = "Hello World";
console.log((str[1]);
for(let lett of str){
	console.log(lett);
}
```

---
### String Length
```javascript
let str = "Hello World";
console.log(str.length);
```

---
### Check String
```javascript
let str = "Hello World JavaScript";
console.log(str.includes("JavaScript"));
console.log(!str.includes("Python"));

if(str.includes("JavaScript)){
				
}
if(!str.includes(Python)){

}
```

---
### Slicing String
```javascript
let str = "Hello Python World String"

console.log(str.slice(2,6)) //slice position to position

console.log(str.slice(0,6)) //slice start to position

console.log(str.slice(6)) //slice position to end

console.log(str.slice()) //slice start to end




```

---
### Upper Case
```javascript
let str = "Hello Python World";
console.log(str.toUpperCase())
```

---
### Lower Case
```javascript
let str = "Hello Python World";
console.log(str.toLowerCase());
```

---
### Remove Whitespace
```javascript
let str = "                    Hello Python World           ";
console.log(str.trim());
```

----
### Replace String
```javascript
let str = "Hello Python World";
console.log(str.replace("World","Programmer"));
```

---
### Split String
```javascript
let str = "Hello Python World";
console.log(str.split(" "));
```

---
### String Concatenate
```javascript
let str1 = "Hello";
let str2 = "World";
print(str1 + " " + str2);
```

---


--- end-multi-column


