- # Exception Handling
- ### Try Except
- The ==try== block lets you test a block of code for errors.
- The ==except== block lets you handle the error.
- The ==else== block lets you execute code when there is no error.
- The ==finally== block lets you execute code, regardless of the result of the try- and except blocks.
```python
try:
	print(x)
except:
	print("There was an error")
```
- ### Many Exception
- You can define as many exception blocks as you want, if you want to execute a special block of code for a special kind of error:
```python
x = 4
try:
	print(x+"")
except NameError:
	print("Not defined X")
except TypeError:
	print("Type not matched")
except SyntaxError:
	print("Syntax is not correct")
except IndexError:
	print("Index out of range")
except KeyError:
	print("Key is not defined")
except:
	print("default error")

```
- ### try
- Execute if no raise error.
```python
try:
	print(4+5)
```
- ### except
- Execute if errors occured
```python
try:
	print(4+"")
except:
	print("Error occured")
```
- ### Else
- Execute if no raise error.
```python
x = 4
try:
	print(4+4)
except:
	print("Something went wrong")
else:
	print("There is no error")
```
- ### Finally
- Execute raise or not raise error.
```python
x = 4
try:
	print(4+4)
except:
	print("Something went wrong")
else:
	print("There is no error")
finally:
	print("Try_Catch block finished")
```

- # Raise or Throw an Error
- To throw or raise an exception, use the ==raise== keyword.
```python
x = int(input("Enter a number"))
if x > 10:
	raise Exception("Sorry, no numbers below zero")
else:
	print("ok")
```
- ### Catch Error Message
```python
x = int(input("Enter a number"))
try:
	if x > 10:
		raise Exception("Sorry, no numbers below zero")
except Exception as msg:
	print(msg)
```

