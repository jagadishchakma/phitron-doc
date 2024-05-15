- # Class
- A Template for making objects.
- Class component: attributes, methods, constructor(instance attribute, instance method). 
```python
class Person:
	pass
```
- ### class attributes (static variable)
- Class attributes are variables that belong to the class itself, not to any individual instance, and are shared across all instances of the class.
```python
class Person:
	name = "Person Guru"

print(Person.name)
```

- ### class methods 
- Class methods are functions defined within a class that operate on class attributes and are accessible by all instances of the class.
```python
class Person:
	name = "Person Guru"
	@classmethod
	def get_name(cls):
		return cls.name
Person.get_name()
```
- ###### "cls" parameter
- The cls parameter in a class method refers to the class itself, allowing the method to access class attributes and create instances of the class.
```python
class Person:
	name = "Person Guru"
	@classmethod
	def get_name(cls):
		return cls.name
```
- ### Static Method
- Static methods are functions defined within a class that operate on class attributes and are accessible by all instances of the class.
- static methods is like class method. but not have self,cls default parameter.
```python
class Person:
	name = "Person Guru"
	@staticmethod
	def get_name():
		return __class__.name
```

- ### Class attributes  or mehtod access or  ==update== inside class:
```python
class Person
	name = "Person Guru"
	def person_name(self):
		return __class__.name
	# or
	def get_person_name(self):
		return Person.name
```


- ### constructor
- A constructor is a special method in object-oriented programming that initializes a newly created object and is automatically called when an object is created
```python
class Person:
	def __init__(self):
		pass
```
- ###### instance attributes
- Instance attributes are variables specific to each object instance of a class, holding data unique to that object
```python
class Person:
	def __init__(self, name):
		self.p_name = name
p1 = Person("Person 1")
print(p1.p_name)
```
- ###### instance methods
- An instance method is a function within a class that operates on instance attributes and is called on an individual object instance.
```python
class Person:
	def __init__(self, name):
		self.p_name = name
	def get_name(self):
		return self.p_name
p1 = Person("Person Guru")
p1.get_name()
```
- ###### "self" parameter
- The self parameter is a reference to the current instance(object) of the class, used to access variables that belong to the class or set attributes to the instance object.
```python
class Person:
	name = "Person Guru"
	def get_name(self):
		return self.name
```

```python
class Person
		def __init__(self)
			pass
p1 = Person()
# p1 === self (just self is memory reference of p1)
# p1.name = "Person Guru" === self.name = name
```

- # Object
- It is an instance of class.
```python
class Person:
	def __int__(self, name):
		self.name = name

p1 = Person("Person 1")
p2 = Person("Person 2")
```
- Python object built in method: dir(),\_\_dict__, \_\_str()__, \_\_repr()\_\_
```python
class Person:
	def __init__(self, name):
		self.name = name
p1 = Person("Person 1")
print(p1.__dict__)
print(dir(p1))
```
- ==Check Object Instance==
- Check object instance using ==isinstance()==
```python
class Person:
	def __init__(self,name):
		self.name  = name
class Engineer:
	def __init__(self, name):
		self.name = name
p1 = Person("John")
p2 = Engineer("Doe")
print(isinstance(p1,Engineer))
print(isinstance(p2,Engineer))
```
- # Class Import
- Class import for reuse code
```python
from book import Book
b1 = Book()
```

```python
import book
b1 = book.Book()
```
- # Pass by Object Reference
- Pass a parameter as a object
```python
class Cat:
	def __init__(self,color,action):
		self.color = color
		self.action = action
	def view(self):
		print(f"Cat color is: {self.color}, Cat action is: {self.action}")
	def compare(self,ct):
		if self.action === ct.action:
			print(f"They are same, {self.action}")
		else:
			print("They are different!!!")

c1 = Cat("White", "Jumphing")
c2 = Cat("Brown", "Sitting")
c2.compare(c1) #pass by reference
```

- # Overloading
- ### Method Overloading
- Method overloading refers to the ability to define multiple methods with the same name but different parameters in a single class.
- Python built in not support method overloading
- But you can achive this using a package: multipledispatch
```python
from multipledispatch import dispatch
class Calculator:
	@dispatch(int,int)
	def add(self, num1, num2):
		cal = num1 + num2
		print(cal)
	@dispatch(int,int,int)
	def add(self, num1, num2, num3):
		cal = num1 + num2 + num3
		print(cal)
	@dispatch(int, int, int, int)
	def add(self, num1, num2, num3, num4):
		cal = num1 + num2 + num3 + num4
		print(cal)

cal1 = Calculator()
cal1.add(1,2)
cal1.add(1,2,3)
cal1.add(1,2,3,4)
```

- ### Constructor Overloading
- Constructor overloading uses different variant of parameter.
- In python built in not support constructor overloading.
- Achive this using \*args.
```python
class Student:
	def __int__(self, *krgs):
		if len(krgs) == 3:
			self.name  = name
			self.id  = id
			self.cgpa = cgpa
		if len(krgs) == 2:
			self.name = name
			self.id = id

s1 = Studen("Jagadish Chakma", 2332, 2.23)
s2 = Student("Namita Chakma", 231)
```

- # 4 Pillars of OOP
- ### Inheritance
- Inheritance in object-oriented programming (OOP) is a mechanism where a new class is created from an existing class, inheriting its properties and behaviors while allowing for additional or modified features.
- Child class can access all properties from parent class but does not do parent class.
- ###### Inheritance Process: ==First Search Child Class If not Found Then Search Parent Class Any.==
- ###### Check Is Subclass:
- Check a class is that subclass or not
```python
class Animal:
	pass
class Cat(Animal):
	pass
print(issubclass(Cat,Animal))
```
- ##### super()
- It's refers the parent class inside the subclass.
```python
class Animal:
	def __init__(self, name):
		self.name = name
	def get_name(self):
		return self.get_name

class Dog(Animal):
	def __init__(self, name, food):
		super().__init__(name) 
		#or
		Animal.__init__(self, name)
		#call a method
		Animal.get_name(self)
		super().get_name() # when call using super() don't need self parameter
```


- ###### super/parent/base class
- A parent class, also known as a superclass or base class, is a class in object-oriented programming (OOP) from which other classes, known as child classes or subclasses, derive. It encapsulates common attributes and behaviors that can be inherited by its subclasses
- ###### sub/child/derived class
- A child class, also known as a subclass or derived class, in object-oriented programming (OOP), is a class that inherits properties and behaviors from another class, referred to as the parent class or base class.
- ###### Types of Inheritance
- Single Inheritance: In which there is one base class and one derived class. 
```python
class Animal: # base class
	pass
class Dog(Animal): # derived class
	pass
```

- Multiple Inheritance: A class can be derived from more than one base classes.
```python
class A:
    def details(self):
        print("From A")
  
class B:
    def details(self):
        print("From B")

class C(A,B):
    def details(self):
       super().details() # using super() not necessary pass self
       print("From C")
       B.details(self) # using class name necessary pass self

o1 = C()
o1.details()
```
- ==Ineritance or finding maintain level up order==

- Multilevel Inheritance: We can inherit a derived class from another derived class.
```python
class GrandFha:
    def __init__(self, name, born):
        self.name = name
        self.born = born
    def details(self):
        print(f"Name is: {self.name}, Born on: {self.born}")
    def live(self):
        print("Not living")

class Father(GrandFha):
    def live(self):
        print("half living")

class Son(Father):
    def live(self):
        print("Fullly living")

s1 = Son("Battey Chakma", 1997)
s1.details()
s1.live()
```

- Hybrid Inheritance: Hybrid inheritance involves multiple inheritance taking place.
```python
class Parent1:
    def method1(self):
        print("method 1 from parent 1")

class Parent2:
    def method2(self):
        print("method 2 from parent 2")

class Child1(Parent1, Parent2):
    def method3(self):
        print("method 3 from child 1")

class Child2(Child1):
    def method4(self):
        print("method 4 from child 2")

obj = Child2()
obj.method1()
obj.method2()
obj.method3()
obj.method4()
```

- Hierarchical Inheritance: In which there is single base class and multiple derived class.
```python
class Student:
    def __init__(self, name, id):
        self.name = name
        self.id = id
    def details(self):
        print(f"Name: {self.name}, ID: {self.id}")
        
class CSEStudents(Student):
    def __init__(self, name, id, labs):
        super().__init__(name, id)
        self.labs = labs
    def cry(self):
        print(f"CSE Student crying because of: {self.labs} labs")

class BBAStudent(Student):
    def enjoy(self):
        print("BBA Student Always do party!!!")

cse = CSEStudents("Jagadish Chakma", 323, 4)
bba = BBAStudent("Namita Chakma", 2332)
cse.cry()
bba.enjoy()
```
- ### Encapsulations
- Encapsulation is the object-oriented programming process that combines attributes and the methods manipulating that data into a single entity, typically a class, to shield its details from external access.
- ###### private
- A private attribute or method is one that is accessible only within its own class and not from outside or derived classes.
- In python use double underscore prefix for private data or method.  
```python
class User:
	def __init__(self, fname, lname, email, password):
		self.fname = fname
		self.lname = lname
		self.email = email
		self.__password = password #private attribute
	def __update_password(self,new_password): # private method
		self.__password = new_password
```
- ###### protected
- A protected attribute or method is one that is accessible within its own class, subclasses, and classes in the same package.
- In python use single underscore prefix for protected data or mehthod
```python
class User:
	pass
```
- ###### public
- public attribute or method is one that can be accessed from any part of the program, as well as from outside the program.
- In python normal method or attribute are also public.
```python
class User:
	def __init__(self, fname, lname, email, password):
		self.fname = fname #public
		self.lname = lname #public
		self._email = email #protected
		self.__password = password #private
```

- ###### Getter and Setter 
- Getters and setters are methods that allow controlled access to the properties of an object, with getters retrieving the value and setters updating it, often with validation.
```python
class User:
	def __init__(self, fname, lname, email, password):
		self.fname = fname #public
		self.lname = lname #public
		self._email = email #protected
		self.__password = password #private
	def get_password(self):
		return self.__password
		@get_password.setter
	defn set_password(self, new_password):
		self.__passwrod = new_password
```

- ### Polymorphism
- Polymorphism means one thing can take many forms.
- ###### Variable Overriding
```python
class Parent:
    def __init__(self) -> None:
        self.house_holder_name = "GrandFa" # override this variable

class Child(Parent):
    def __init__(self, name) -> None:
        self.house_holder_name = name

c1 = Child("Jagadish Chakma")
print("House Holder Name: ", c1.house_holder_name)
```
- ###### Method Overriding
```python
class GrandFa:
    def advice(self): # override this method
        print("Always do hard working!!!")

class Child(GrandFa):
    def advice(self):
        print("Always do party!!!")

c1 = Child()
c1.advice()
```

- ### Abstraction
- Abstract can be considered as a blueprint for other classes.
- Abstract provides common attributes and methods for all subclasses for reduction of code.
- Abstract contains one or more abstract methods.
- We use abstract class when we design large functional units.
- Python does not provide abstract classes by defult.
- ==An abstract class is not a concrete class, it cannot be instantiated.==
- ==Abstract method has not body.==
```python
from abc import ABC,abstractmethod
class GrandFa(ABC):
	@abstractmethod
	def must_be_savings(self):
		print("savings the money")
		
class Father(GrandFa):
	@abstractmethod
	def must_be_study(self):
		print("must be study")

class Son(Father):
	def must_be_savings(self):
		print("Yes, I do savings")
	def must_be_study(self):
		print("Yes, I do study")
```


