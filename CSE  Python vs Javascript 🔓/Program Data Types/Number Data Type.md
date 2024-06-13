

--- start-multi-column: ID_69e9
```column-settings
Number of Columns: 2
Largest Column: standard
```

# <p align="center">integer, float, complex</p>

---
### ==integer,float,complex== are object their have own properties and methods.
```python
print(dir(23))
```

---
### integer
- Int, or integer, is a whole number, positive or negative, without decimals, of unlimited length.
```python
short = 123
long = 3243243242
```

---
### float
- Float, or "floating point number" is a number, positive or negative, containing one or more decimals.

```python
short = 123.323
long = -2313.2324
```

- Float can also be scientific numbers with an "e" to indicate the power of 10.
```python
short = 35e3  
long = 12E4
```

---
### complex
- Complex numbers are written with a "j" as the imaginary part.
```python
x = 3+5j  
y = 5j  
z = -5j
```

---
### Type Casting
```python
num1 = int() #convert any number to integer
num2 = float() #convert any number to floating point
num3 = complex() #convert only integer to complex
str_num = str(123) #conver number to string












```

<br>

---
### Random Number
```python
import random
ranNum = random.randint(1,20)
print(ranNum)
```

---
### Methods
- Becaue python number is not an object.
- To achive like this functionality describe below

```python


str(213)
format(123.2323,'.2f')






int(13.23)
float(2312)
```

--- column-break ---

# <p align="center">number</p>

---
### ==number== is object this have own properties and methods.
```python
console.dir(new Number(3))
```

---


- number is included all type of integer, float,complex.

<pre>


</pre>

```javascript
let short = 123;
let long = 3243243242
```

<pre>





</pre>

```javascript
let short = 123.323;
let long = -2313.2324;
```

- Extra large or extra small numbers can be written with scientific (exponent) notation

```javascript
let short = 35e3;
let short = 12E4;
```

<pre>













</pre>

---
### Type Conversion
```javascript
// string,boolean to number conversion
let num = Number("123");
let num = +"123";
let num = parseInt("123");
let num = parseFloat("123");
let num = Number(true);
let num = Number(false);

// number to string,boolean
let str = String(123);
let str = (123).toString()
let bool = Bool(1);
let bool = Bool(0);
let bool = !!1; // use negation



```

---
### Random Number
```javascript
let ranNum = Math.floor(Math.random()*19) // 0-19 random number
let ranNum = Math.floor(Math.random() * (max - min + 1) + min)) // including min max both
let ranNum = Math.floor(Math.random() * (max - min ) + min)) // not including max
```

---
### Number methods
- As javascript any number behind the refer a Number constructor that's why a number is an object and as a object have some methods and propertis.
- number constructor = new Number()
```javascript
//local methods
2133.toString() // number to string convert
1233.toFixed(2) // decimal number how many specified
1233.toPrecision(3) // number digits specified

//global methods
isNaN()
Number.isInteger()
isFinite()
parseInt()
parseFloat()
```

--- end-multi-column

