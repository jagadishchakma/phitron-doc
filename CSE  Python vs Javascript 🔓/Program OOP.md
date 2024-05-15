

--- start-multi-column: ID_fcvu
```column-settings
Number of Columns: 2
Largest Column: standard
```

# <p align="center">Python</p>

---
### Classes
```python
class MyClass:
	pass
	
```

---
### Object
```python
obj = MyClass()
```

---
### Constructor
```python
class MyClass:
	def __init__(self):
		pass


```

---
### Class Variable
```python
class MyClass:
	admin_name = "Jagadish Chakma"

print(MyClass.admin_name)
```

---
### Class Method
```python
class MyClass:
	admin_name = "Jagadish Chakma"
	@classmethod
	def myfunc(cls):
		return cls.admin_name

print(MyClass.myfunc())



```

--- 
### Self Keyword
```python
class MyClass:
	def __init__(self):
		self.fname = "Jagadish",
		self.lname = "Chakma"
	def myfunc(self):
		print(self.fname,self.lname)



```

---
### Inheritance
- support single, multi-level, hierarchical,multiple,hybrid inheritance.
```python
class Class1:
	pass

class Class2:
	pass

class Class3:
	pass


class Class4(Class1,Class2, Class3):
	pass
```

---
### super() method
- access parent class original property as well constructor.
```python
class Class1:
	def __int__(self, title):
		self.title = title

class Class2:
	def __int__(self, title):
		self.title = title

class Class3:
	def __int__(self, title):
		self.title = title


class Class4(Class1,Class2, Class3):
	def __int__(self, title1, title2, title3):
		super().__init__(title1)
		Class2.__init__(slef, title2)
		Class3.__init__(self, title3)
```

---
### Abstraction
- hides an application's internal details from the outside world.
- parent pre-defined command for child.
```python
from abs import ABC, abstractmethod

class Parent(ABC):
	@abstractmethod
	def married(self):
		pass
	@abstracmethod
	def doSavings(self):
		pass

class Child(Parent):
	def married(self):
		print("Yes, Married")
	def doSavings(self):
		print("Yes, Savings")


```

---
### Polymorphism
```python
class Animal:
	def sound():
		print("Animal is loughing")

class Dog(Animal):
	def sound():
		print("Dog is geu geu kore")

class Cat(Animal):
	def sound():
		print("Cat is meu meu kore")






```

---
### Encapsulation
```python
class MyClass:
	def __init__(self):
		self.__salary = 230000
	def ___transaction(self):
		pass



```
--- column-break ---

# <p align="center">JavaScript</p>

---
### Classes
```javascript
class MyClass{

}
```

---
### Object
```javascript
obj = new MyClass()
```

---
### Constructor
```javascript
class MyClass{
	constructor(){
	
	}
}
```

---
### Class Variable
```javascript
class MyClass{
	static admin_name = "Jagadish Chakma";
}
console.log(MyClass.admin_name);
```

---
### Class Method
```javascript
class MyClass{
	static admin_name = "Jagadish Chakma";
	static myfunc(){
		return MyClass.admin_name;
	}
	constructor(){
	
	}
}
console.log(MyClass.myfunc())
```

---
### this keyword
```javascript
class MyClass{
	constructor(){
		this.fname = "Jagadish";
		this.lname = "Chakma";
	}
	myfunc(){
		console.log(this.fname, this.lname);
	}
}
```

---
### Inheritance
- support only single inheritance.
```javascript
class Parent{
	
}

class Child extends Parent{

}





```

---
### super() method
- call parent class constructor.
```javascript
class Parent{
	constructor(title){
		this.title = title
	}
}

class Child extends Parent{
	constructor(headline){
		super(headline);
	}
}







```

---
### ==Not Have== But User Defined Have
- hides an application's internal details from the outside world.
- ==Not Have==
```javascript
class Parent{
	marriend(){
	}
	doSavings(){
	}
}

class Child extends Parent{
	married(){
		console.log("Yes, Married");
	}
	doSavings(){
		console.log("Yes, Savings");
	}
}


```

---
### Polymorphism
```javascript
class Animal{
	sound(){
		console.log("Animal is sounding");
	}
}

class Dog extends Animal{
	sound(){
		console.log("Dog sound is geu geu kore");
	}
}

class Cat extends Animal{
	sound(){
		console.log("Cat sound is meu meu kore");
	}
}
```

---
### Encapsulation
```javascript
class MyClass{
	constructor(){
		this.#salary = 23323080
	}
	#transaction(){
		
	}
}
```

--- end-multi-column


