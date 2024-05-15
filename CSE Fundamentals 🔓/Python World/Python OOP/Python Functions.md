- # Define
```python
def my_func():
	pass

my_func()
```
- # Return
- If you no have return python default return "None" data type
```python
def my_func():
	pass

print(my_func())
```
- # Argumetns
- ### Default parameter value
```python
def my_func(title="Second Title"):
	print(title)

my_func()
```
- ### Arbitary Arguments
- Arbitary arguments are recieve as a tuple type.
```python
def my_func(fname,lname, *args):
	for arg in args:
		print(arg)
my_func("jagadish","chakma",27,"rangamati","study")
```
- ### Keyword Arguments
- Keyword arguments for accept don't necessary follow order.
```python
def my_func(fname,lname,age,city,village):
	print(fname,lname,age,city,village)
my_func(city="rangamati", age=27, village = "Bodhipur", fname="Jagadish", lname="Chakma")
```
- ### Arbitary Keyword Arguments
- Arbitary keyword arguments are recieve as a dictionary.
```python
def my_func(fname,lname,**info):
	for key,value in info.items():
		print(key,value)
my_func(city="rangamati", age=27, village = "Bodhipur", fname="Jagadish", lname="Chakma")
```
- ### Anonymous Function
- Can take any number of arguments but have only one expression.
- Automatically expression return it.
- Also called this lambda function.
```python
sum = lambda n1,n2,n3,n4,n5: n1+n2+n3+n4+n5
print(sum(1,2,3,4,5))
```



