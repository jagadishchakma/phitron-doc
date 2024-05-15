

--- start-multi-column: ID_w60h
```column-settings
Number of Columns: 2
Largest Column: standard
```

# <p align="center">Python</p>

---
### Declare:

```python
def myfunc():
	#codeblock here
	
```

---
### Arbitary Arguments:

```python
def myfunc(*args):
	print(args)

myfunc("Jagadish Chakma", 28, "Bodhipur", "BBA", "CSE")
```

```python
def myfunc(name, age, *args):
	print(args)

myfunc("Jagadish Chakma", 28, "Bodhipur", "BBA", "CSE")
```

---
### Arbitary Keywords Arguments:

```python
def myfunc(language,framework,library,popular):
	print(language, framework, library, popular)

myfunc(framework="Django", popular="High", language="Python", library="Flask")
```


### \*\*args
```python
def myfunc(**args):
	print(args)

myfunc(framework="Django", popular="High", language="Python", library="Flask")
```


---
### Lambda Function
- A lambda function is a anonymous function which take any number of argumetns but only have one expression.
```python
myfunc = lambda p1,p2: p1+p2

print(myfunc(21,23))

```

---
### ===Not Have===
```python

























```

---

--- column-break ---

# <p align="center">JavaScript</p>

---
### Declare:

```javascript
function myfunc(){
	//codeblock here
}
```

---
### Rest Operator:

```javascript
function myfunc(...params){
	console.log(params)
}
myfunc("Jagadish Chakma", 28, "Bodhipur", "BBA", "CSE")
```

```javascript
function myfunc(name, age, ...params){
	console.log(params)
}
myfunc("Jagadish Chakma", 28, "Bodhipur", "BBA", "CSE")
```

---
### Arbitary Keywords Arguments:

```javascript
function myfunc(language,framework,library,popular):
	console.log(language, framework, library, popular)

myfunc(framework="Angular", popular="High", language="JavaScript", library="React")
```

### ==Not Have==


```javascript




```


---
### Anonymous Function:
- An anonymous function is a function without a name.
```javascript
let myfunc = function(p){
	console.log(p);
}
myfunc("Hello")
```

---

### Arrow Function:
- An arrow function is a function that allows for a shorter syntax and does not have its own ==this==, ==arguments==, and ==super==, and cannot be used as constructor.
```javascript
let myfunc = () => {
	
}
```


### Arrow Vs Normal Functions:
- Syntax
- this binding
- arguments object
- constructors
- method definitions

--- end-multi-column



