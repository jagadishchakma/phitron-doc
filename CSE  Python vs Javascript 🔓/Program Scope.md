

--- start-multi-column: ID_hxls
```column-settings
Number of Columns: 2
Largest Column: standard
```

# <p align="center">Python</p>

---
### Local Scope
- A variable created inside a function belongs to the local scope of that function, and can only be used inside that function.
```python
def myfunc():
	language = "Python"
	print(language)
print(language)#not possible access and get error

```

---
### Global Scope
- A variable created in the main body is called a global scope. Global variable can access both side.
```python
language = "Python"
def myfunc():
	print(language)
print(language)

```

---
### ==Not Have==
```python








```

---
### Global Keyword
- Make a local variable to global variable using global keyword.
```python
def myfunc():
	global language
	language = "Python"
print(language)
```
--- column-break ---

# <p align="center">JavaScript</p>

---
### Local Scope
- A variable created inside a function belongs to the local scope of that function, and can only be used inside that function.
```javascript
function myfunc(){
	var language = "JavaScript";
	console.log(language);
}
console.log(language)//not possible access and get error
```

---
### Global Scope
- A variable created in the main body is called a global scope. Global variable can access both side.
```javascript
var language = "JavaScript";
function myfunc(){
	console.log(language);
}
console.log(langugae);
```

--- 
### Block Scope
- let or const are declared inside the {} curly braces is called block scope. Block scope variables are only accessible inside block not outside.
```javascript
if(true){
	let language = "JavaScript";
	console.log(language);
}
console.log(language); // gettting an error
```

---
### ==Not Necessary== Because JS Have Assigning System
```javascript
var language;
function myfunc(){
	language = "JavaScript"
}
console.log(language)


```

--- end-multi-column
