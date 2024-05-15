- # Local Scope
- A variable created inside a function is called local scope.
```python
def my_func():
	x = 10
	print(X)
my_func()
```
- Local variable only use inside function.
- # Global Scope
- A variable created outside a function is called global scope.
```python
x = 10
def my_func():
	print(x)
my_func()
```
- Global variables are  accessible from all of the side.
- # Global Keyword
- The ==global== keyword makes the variable global.
```python
def my_func():
	global x
	x = 19
my_func()
print(x)
```
- # Nonlocal Keyword
- The ==Nonlocal== keyword makes the variable belong to the outer function.
```python
def my_func():
	def my_fun2():
		nonlocal x
		x = 30
	print(x)
```
