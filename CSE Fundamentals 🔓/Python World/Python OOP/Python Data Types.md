# Data Types:
- Text type: ==str==
- Numeric types: ==int==, ==float==, ==complex==
- Sequence types: ==list==, ==tuple==, ==range==
- Mapping types: ==dict==
- Set types: ==set==, ==frozenset==
- Boolean type: ==bool==
- Binary types: ==bytes==, ==bytearray==, ==memoryview==
- None type: ==None==
# Define Data Types:
- ==str==
```python
my_var = "Hello Python"
my_var = 'Hello Python'
```
- ==int==
```python
my_var = 20
```
- ==float==
```python
my_var = 20.20
```
- ==complex==
```python
my_var = 1j
```
- ==list==
```python
my_var = ["apple", "banana", 20]
```
- ==tuple==
```python
my_var = ("apple", "banana", 20)
```
- ==range==
```python
my_var = range(6)
```
- ==dict==
```python
my_var = {"name": "john", "age": 20}
```
- ==set==
```python
my_var = {"apple", "banana", 20}
```
- ==frozenset==
```python
my_var = ({"apple", "banana", 20})
```
- ==bool==
```python
my_var  = True
my_var = False
```
- ==None==
```python
my_var = None
```
# Check Data Types
- To check data types use ==type()==
```python
my_var = "Hello Python"
print(type(my_var))
```


<hr>

# String Data Types:
- ### Strings
- Strings in python are surrounded by either single quotation marks, or double quotaion marks.
```python
my_var = "Hello World"
my_var = 'Hello World'
```
- ### Quotes Inside Quotes
- You can use quotes inside a sring, as long as they don't match the quotes surronding the string:
```python 
my_var = "Hello World of my Girl's"
```
- ### Multiple Strings
- You can assigne multiple string to a variable by using three quotes:
```python
my_var = """multiple string.
multiple string
multiple string
"""
```
- ### Strings are Arrays
- Like another popular programming language string threaded as arrays.
```python
my_var = "Hello Python"
print(my_var[3])
#or looping string as like array
for item in my_var:
	print(item)
```
- ### String Length
- To get the length of a string, use the ==len()== function.
```python
my_var = "Hello Python"
print(len(my_var))
```
- ### Check String
- To check if a certain phrase or character is pressent in a string, we can use the keyword ==in== 
```python
my_var = "Hello Python Codig Lover"
check = "Coding" in my_var
print(check)
```
- ### Check If Not
- To check if a certain phrase or character is NOT present in a string, we can use the keyword ==not in==
```python
my_var = "Hello Python Coding Lover"
check = "Jagascript" not in my_var
print(check)
```

- ### Slicing
- You can return a range of characters by using the slice syntax.
- Specify the start index and the end index, separated by a colon, to return a part of the string.
```python
my_var = "Hello Python Coding Lover"
print(my_var[2:5:1])
```
- Slice From The Start:
- By leaving out the start index, the range will start at the first character.
```python
my_var = "Hello Python Coding Lover"
print(my_var[:5])
```
- Slice To The End:
- By leaving out the end index, the range will go to the end:
```python
my_var = "Hello Python Coding Lover"
print(my_var[5:])
```
- Slice Frist To Last:
- By leaving out the first,end index, the range will go to the first to last:
```python
my_var = "Hello Python coding Lover"
print(my_var[:])
```

- Negetive Slice:
- By using negetive value end to first , the range will go to the last ot first:
```python
my_var = "Hello Python Coding Lover"
print(my_var[-1:-8:-1])
```
- Reverse String:
- By using negetive leaving middle value reverse a stirng:
```python
my_var = "Hello Python Coding Lover"
print(my_var[-1::-1])
```
- ### String Concatenation
- To concatenate, or combine, two strings you can use the + operator.
```python
string1 = "Hello"
string2 = "Python"
add = string1 + " " + string2
print(add)
```
- ### String Format
- Using F-string we can format  a string
```python
language = "Python"
my_var = f"Hello {language} Coding Lover"
print(my_var)
```
- ### String Escape Characters
- We can use escape character in string
```python
my_var = "Hello\t Python\n \\Coding Lover\"s"
print(my_var)
```
- String Constructor
```python
string = ("i am string")
```
- ### Add String to String
- Join multiple strings
```python
fname = "Jagadish"
lname = "Chakma"
fname += lname
print(fname)
```
- ### Unpacking String
- like javascript destructuring
```python
name = "Jhon Doe"
a, b, *c = name
print(a,b)
```




- ### String Methods
- Upper Case:
- The ==uper()== method returns the string in upper case.
```python
my_var = "Hello Python"
print(my_var.upper())
```
- Lower Case:
- The ==lower()== method returns the string in lower case.
```python
my_var = "Hello Python"
print(my_var.lower())
```
- Remove White Space:
- White space is the space before and / or after the actual text. Remove using ==strip()==
```python
my_var = " Hello Python         "
print(my_var.strip())
```
- Replace String:
- The ==replace(target_string, replace_string)== method replaces a string with another string.
```python
my_var = "Hello Python"
print(my_var.replace("H", "P"))
```
- Split String:
- The ==split()== method returns a list where the text between the specified separator becomes the list item.
```python
my_var = "Hello, Python, Coding , Lover"
print(my_var.split(","))
```
- String Capitalize:
- Upper case the first letter using ==capitalize()==.
```python
my_var = "Hello Python"
print(my_var.capitalize())
```
- String casefold()
- Convert strings into lowercase using ==casefold()==
```python
my_var = "Hello Python Coding Lover"
print(my_var.casefold())
```
- String center():
- Returns a  centered string
```python
my_var = "Hello Python"
print(my_var.center(10))
```
...........................................................................loading..............
<hr>

# Number Data Types
- ### Types
- int
- float
- complex
- ### Type Conversion
- You can not convert complex number another type.
```python
a = 21
b = 23.32
c = 3j
print(float(b))
print(int(a))
print(complex(a))
```
- ### Random Number
- Python does not have built in random function to make a random number, but python has a built in module called ==random== that can be used to make random numbers.
```python
import random
print(random.randrage(0,10))
```
- ### Number Constructor
```Python
integer = int(23)
floatingpoint = float(234.34)
complexnum = complex(2j)
```
# List Data Type
- List are used to store multiple items in a single variable.
- List items are ordered, changable, and allow duplicate values.
- List items are indexd, the first item has index[0], the second item has index [1].
- List items can be any of data types.
```python
my_var = ["JavaScript", "PHP", "Python", "C", "C++", "Java"]
```
- ### The list() Constructor
- It is also possible to use the ==list()== constructor when creating a new list.
```python
my_var = list(("JavaScript","PHP", "Python", "c", "c++", "Java"))
```
- note that double rounded brackets.
- ### List Length
- To determine how many items a list has , use the ==len()== function.
```python
my_var = ["JavaScript", "PHP", "Python", "C", "C++", "Java"]
print(len(my_var))
```
- ### Access List Items
```python
my_var = ["JavaScript", "PHP", "Python", "C", "C++", "Java"]
print(my_var[0])
```
- ### Range of Indexes
```python
my_var = ["JavaScript", "PHP", "Python", "C", "C++", "Java"]
print(my_var[2:4])
```
- steps skip:
```python
my_var = ["JavaScript", "PHP", "Python", "C", "C++", "Java"]
print(my_var[0:4:2])
```
- first to range:
```python
my_var = ["JavaScript", "PHP", "Python", "C", "C++", "Java"]
print(my_var[:4])
```
- range to end:
```python
my_var = ["JavaScript", "PHP", "Python", "C", "C++", "Java"]
print(my_var[2:])
```
- Negetive Indexes:
- Index start from -1
- end to range:
```python
my_var = ["JavaScript", "PHP", "Python", "C", "C++", "Java"]
print(my_var[:-4:-1])
```
- range to first:
```python
my_var = ["JavaScript", "PHP", "Python", "C", "C++", "Java"]
print(my_var[-3::-1])
```
- end to first
```python
my_var = ["JavaScript", "PHP", "Python", "C", "C++", "Java"]
print(my_var[::-1])
```
- ### Check
- check a value that exists in list using ==in==
```python
my_var = ["JavaScript", "PHP", "Python", "C", "C++", "Java"]
check = "PHP" in my_var
print(check)
```
- check a value that not exists in list using ==not in==
```python
my_var = ["JavaScript", "PHP", "Python", "C", "C++", "Java"]
check = "php" no in my_var
print(check)
```
- ### Change Item Value
- To change the value of a specific item, refer to the index number.
```python
my_var = ["JavaScript", "PHP", "Python", "C", "C++", "Java"]
my_var[3] = "Ruby"
print(my_var)
```
- Change a range of item:
```python
my_var = ["JavaScript", "PHP", "Python", "C", "C++", "Java"]
my_var[2:4] = ["Django", "Laravel"]
print(my_var)
```
- ### List Constructor
```python
mylist = list(1,2,3)
```
- ### Iterate List Item
```python
language = ["javascript", "python", "php", "java"]
for item in language:
	print(item)
```
- ### Add List to List
- Join multiple lists
```python
list1 = [1,2,3,4]
list2 = [5,6,7]
list1 += list2
print(list1)
```
- ### Unpacking List
- like javascript destructuring
```python
numbers = [1,2,3,4,5]
a,b,c,*d = numbers
print(a,b,c)
```


- ### List Methods
- ==insert()
- Insert Items:
- To insert a new list item, without replacing any of the existing values, we can use the ==insert()== mehtod.
```python
my_var = ["JavaScript", "PHP", "Python", "C", "C++", "Java"]
my_var.insert(0,"Go")
print(my_var)
```
- ==append()==
- Append Items:
- To add an item to the end of the list, use the ==append()== method:
```python
my_var = ["JavaScript", "PHP", "Python", "C", "C++", "Java"]
my_var.append("Ruby")
print(my_var)
```

- ==extend()==
- Extend List:
- To append elements from another list to the current list, use the ==extend== method
```python
language = ["JavaScript", "PHP", "Python", "C", "C++", "Java"]
framework = ["Django", "Flask", "Laravel", "React"]
language.extend(framework)
print(language)
```
- # Tuple Data Type
- Tuples are used to store multiple items in a single variable.
- A tuples is a collection  which is ordered and unchangable and allow duplicate value.
- Tuple are writen using curly brackets.
```python
language = ("javascript", "php", "pytho", "c", "c++")
```

- ### Items
- Tubple items are ordered, unchangeable, and allow duplicate values.
- Tuple items are indexed, the first item has index [0], the second item has index [1]
```python
language = ("javascript", "php", "python", "c", "c++")
print(language[0])
print(language[3])
```
- ### Ordered
- When we say that tuples are ordered, it means that the items have a defined order, and that order will not change.
- ### Unchangeable
- Tuples are unchangeable, meaning that we cannot change, add or remove items after the tuple has been created.
```python
language = ("javascript", "php", "python", "ruby")
language[0] = "swift" ## getting an error
```
- ### Allow Duplicate
- Since tuples are indexed, they can have items with the same value:
```python
language = ("javascript", "java", "php", "python", "ruby", "javascript")
print(language)
```
- ### Tuple Length
- To determine how many items a tuple has, use the ==len()== function:
```python
language = ("javascript", "java", "php", "python", "ruby", "javascript")
print(len(language))
```
- ### Create Tuple With One Item
- To create a tuple with only one item,  you have to add a comma after the item, otherwise Python will not recognize it as  a tuple.
```python
language = ("javascript",)
print(type(language))
framework = ("django")
print(type(framework))
```
- ### Tuple Items Data Type
- A tuple can contain different data types:
```python
javascript = ("programming language", 1997, "Brendan Ick", True)
print(javascript)
```
- ### Tuple Constructor
```python
mytuple = tuple("javascript", "php")
```
- ### Tuple Value Check
- Tuple value check using ==in== or ==not in== 
```python
language = ("javascript", "php", "ruby", "python")
userInput = input("Enter input langue:")
if userInput in language:
	print("found")
else:
	print("not found")

if userInput not in language:
	print("Yes not have)
else:
	print("sorry, have")
```
- ### Iterate Tuple Items
```python
languge  = ("javascrit", "php", "Python")
for item in language:
	print(item)
```
- ### Tuple Range Items
- Tuple iterating accept positive or negetive indexing.
```python
language = ("javascript", "php", "python", "java")
print(language[:3]) # positive indexing
print(language[::-1]) # reverse items
```
- ### Change Tupple Values Even If Unchangeable
- Follow a technic
```python
language = ("javascript", "php", "python", "java")
l1 = list(language)
l1[0] = "java"
language = tuple(l1)
print(language)
```
- ### Add Tuple to Tuple
- Join multiple tuples
```python
language = ("javascript", "php")
framework = ("django", "node", "laravel")
language += framework
print(language)
```

- ### Unpacking Tuple
- like javascript destructure
```python
language = ("Javascript", "php", "java", "c++")
a,b,*c = language
print(a,b,c)
```
- ### Tuple Methods
- ###### count()
- returns the number of times a specified value occurs in a tuple.
```python
numbers = (1,2,3,4,5,2,1,3,4,2,2,3)
print(numbers.count(2))
```
- ###### index()
- searches the tuple for a specified value and returns the position.
```python
number = (1,2,3,3,4,4,5)
print(number.index(3))
```

- # Set Data Types
- Sets are used to store multiple items in a single variable.
- A Set is a collection which unordered, unchangeable, and unindexed, and not allowed duplicate values.
- Sets are written with curly brackets.
```python
booksets = {"Dhammapad", "Jataka", "Binoy Pitaka"}
```

- ### Set Items
- Set items are unordered, unchangeable, unindex, and not allowed duplicate values.
- ### Unordered
- Unordered means that the items in a set do not have a defined order.
- Set items can appear in a different order every time you use them,  and cannot be referred to by index or key.
- ### Unchangeable
- Set items are unchangeable, meaning that we cannot change the items after the set has been created.
- Once  a set is created, you cannot change its items, but you can remove items and new items.
- ### Duplicates Not Allowed
- Duplicates values will be ignored.
```python
booksets = {"Dhammapad", "Jataka", "Binoy Pitaka", "Jataka"}
print(booksets)
```
- The value ==True== and ==1== are considered the same value in sets, and are treated as duplicates
- The value ==False== and ==0==  are considered  the same value in sets, and are treated as duplicates.
```python
booksets = {"Dhammapad", "Jataka", "Binoy Pitaka", "Jataka", True, 1, False, 0}
print(booksets)
```

- ### Get The Length
- To determine how many items a set has, use the ==len()== function
```python
booksets = {"Dhammapad", "Jataka", "Binoy Pitaka", "Jataka", True, 1, False, 0}
print(len(booksets))
```
- ### Items Data Types
- Set items can be of any data type
```python
booksets = {"Dhammapad", "Jataka", "Binoy Pitaka", "Jataka", True, 1, False, 0}
print(booksets)
```

- ### Access Items
- You cannot access items in a set by referring to an index or a key.
- But you can loop throught the set items using a ==for== loop, or ask if a specified value is present in a set, by using the ==in==  or ==not in== keyword.
```python
booksets = {"Dhammapad", "Jataka", "Binoy Pitaka", "Jataka", True, 1, False, 0}
for item in booksets:
	print(item)

if "Jataka" in booksets:
	print("Found")
else:
	print("Not Found")
```
- ### Change Items
- Once a set is created , you cannot change its items, but you can add new items.
- ### Add Items
- To add one item to a set use the `add()` method.
```python
booksets = {"Dhammapad", "Jataka", "Binoy Pitaka", "Jataka", True, 1, False, 0}
booksets.add("newItem")
```
- ### Add Any Iterable
- Add any iterable object by using ==update()== method.
```python
booksets = {"Dhammapad", "Jataka", "Binoy Pitaka", "Jataka", True, 1, False, 0}
booklists = ["Abidhamma Pitaka", "Bissuddi margo", "Paribar Path"]
booksets.update(booklists)
```
- ### Remove Set Items
- Remove by using ==remove()== ==discard()== 
```python
booksets = {"Dhammapad", "Jataka", "Binoy Pitaka", "Jataka", True, 1, False, 0}
removeItem = input("Enter remove item:")
booksets.remove(removeItem) # if found will raise an error
booksets.discard(removeItem) # if not found will not raise an error

```

- ### Set Constructor
- It is also possible to use the ==set()== constructor to make a set.
- Note that use double curly brackets.
```python
booksets(("Dhammapad", "Jataka", "Binoy Pitaka", "Jataka", True, 1, False, 0))
```

- ### Set Methods
- ............
- # Dictionaries Data Type
- Dictionaries are used to store data values in key:value pairs.
- A dictionary is a collection which is ordered, changeable and do not allow duplicates.
- Dictionaries are written with curly brackets, and have keys and values.
```python
person = {"fname":"Jagadish", "lname": "Chakma", "age": 28, "city": "Rangamati"}
```
- ### Dictionaries Items
- Dictionary items are ordered, changeable,  and do not allow duplicates.
- Dictionary items are presented in key:value paris, and can be referred to by using the key name.
```python
person = {
	"fname":"Jagadish",
	"lname":"Chakma",
	"age":27,
	"city":"Rangamati"
}
print(person["fname"])
```

- ### Ordered or Unordered
- Python latest is ordered.
- Python 3.6 or later are unordered.
- ### Changeable
- Dictionaries are changeable, meaning that we can change, add or remove items after the dictionary has been created.
- ### Duplicates Not Allowed
- Dicrionaries cannot have two items with the same key:
- Duplicate values will overwrite existing values.
```python
person = {
	"fname":"Jagadish",
	"lname":"Chakma",
	"age":27,
	"city":"Rangamati",
	"age": 28
}
print(person["fname"])
```
- ### Dictionary Length
- To determine how many items a dictionary has, use ==len()== function.
```python
person = {
	"fname":"Jagadish",
	"lname":"Chakma",
	"age":27,
	"city":"Rangamati"
}
print(len(person))
```
- ### Dictionary Items Data Types
- The values in dictionary items can be of any data type.
```python
person = {
	"fname":"Jagadish",
	"lname":"Chakma",
	"age":27,
	"city":"Rangamati"
	"Job": False
	"Married": False
	"Study": True
}
print(person)
```

- ### Dictionaries dict() Constructor
- It is also possible to use the ==dict()== constructor to make a dictionary.
```python
person = dict(
		  fname: "Jagadish",
		  lanem: "Chakma",
		  age: 27,
		  city: "Rangamati"
)
print(person)
```
- ### Accessing Items
- You can access the items of a dictionary by referring to its key name, inside square brackets.
```python
person = {
	"fname":"Jagadish",
	"lname":"Chakma",
	"age":27,
	"city":"Rangamati"
	"Job": False
	"Married": False
	"Study": True
}
print(person["age"])
```
- Or you can access by using ==get()== methods
```python
person = {
	"fname":"Jagadish",
	"lname":"Chakma",
	"age":27,
	"city":"Rangamati"
	"Job": False
	"Married": False
	"Study": True
}
print(person.get("age"))
```

- ### Get Dictionaries Keys
- The ==keys()== method will return a list of all the keys in the dictionary.
```python
person = {
	"fname":"Jagadish",
	"lname":"Chakma",
	"age":27,
	"city":"Rangamati"
	"Job": False
	"Married": False
	"Study": True
}
print(person.keys())
```

- ### Get Dictionaries Values
- The ==values()== method will return a list of all values in the dictionary.
```python
person = {
	"fname":"Jagadish",
	"lname":"Chakma",
	"age":27,
	"city":"Rangamati"
	"Job": False
	"Married": False
	"Study": True
}
print(person.values())
```

- ### Check If Key Exists or Not
- Check a key exists or not using ==in== and ==not in==
```python
person = {
	"fname":"Jagadish",
	"lname":"Chakma",
	"age":27,
	"city":"Rangamati"
	"Job": False
	"Married": False
	"Study": True
}
inputkey = input("Enter you find key: ")
if inputKey in person:
	print("Found")
else:
	print("Not Found")

if inputKey not in person:
	print("Yes, not have")
else:
	print("OOps, have")
```
- ### Change Values
- You can change the specific key value by referring key name.
```python
person = {
	"fname":"Jagadish",
	"lname":"Chakma",
	"age":27,
	"city":"Rangamati"
	"Job": False
	"Married": False
	"Study": True
}
updateKey = input("Enter update key")
updateValue = input("Enter update value")
person[updateKey] = updateValue
print(person)
```
- ### Update Items
- You can update existing dictionary keys by using the ==update()== method. If provided key not exist then it will be added.
```python
person = {
	"fname":"Jagadish",
	"lname":"Chakma",
	"age":27,
	"city":"Rangamati"
	"Job": False
	"Married": False
	"Study": True
}
person.update({"Job": True})
print(person)
```
- ### Add Items
- You can add new items by create a key and value assign.
```python
person = {
	"fname":"Jagadish",
	"lname":"Chakma",
	"age":27,
	"city":"Rangamati"
	"Job": False
	"Married": False
	"Study": True
}
person["location"] = "Manikchari"
print(person)
```
- ### Remove Items
- You can remove items from dictionary using ==pop()== method
```python
person = {
	"fname":"Jagadish",
	"lname":"Chakma",
	"age":27,
	"city":"Rangamati"
	"Job": False
	"Married": False
	"Study": True
}
person.pop("fname")
```
- ### Loop Dictionaries
- You can loop through a dictionary using a ==for== loop.
- ###### Loop Keys
```python
person = {
	"fname":"Jagadish",
	"lname":"Chakma",
	"age":27,
	"city":"Rangamati"
	"Job": False
	"Married": False
	"Study": True
}
for key in person.keys():
	print(key)
```
- ###### Loop Values
```python
person = {
	"fname":"Jagadish",
	"lname":"Chakma",
	"age":27,
	"city":"Rangamati"
	"Job": False
	"Married": False
	"Study": True
}
for value in person.values():
	print(value)
```
- ###### Loop Keys Values
```python
person = {
	"fname":"Jagadish",
	"lname":"Chakma",
	"age":27,
	"city":"Rangamati"
	"Job": False
	"Married": False
	"Study": True
}
for key,value in perosn.items()
	print(key,value)
```
- ### Copy a Dictionary
- Copy a dictionary to another dictionary
```python
person = {
	"fname":"Jagadish",
	"lname":"Chakma",
	"age":27,
	"city":"Rangamati"
	"Job": False
	"Married": False
	"Study": True
}
newPerson = person.copy()
```
- ### Nested Dictionary
- A dictionary  can contain dictionaries, this is called nested dictionaries.
```python
person = {
	"fname":"Jagadish",
	"lname":"Chakma",
	"family":{
		"father": "Bijoy Chakma",
		"mother": "kalamila chakma"
	}
	"age":27,
	"city":"Rangamati"
	"Job": False
	"Married": False
	"Study": True
}
print(person)
```
- ### Dictionary Methods
- .............
- 

