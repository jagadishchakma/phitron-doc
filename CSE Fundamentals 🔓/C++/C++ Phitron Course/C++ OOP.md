# Phitron
- Dynamic objcet copy system:
```c++
Person* p1 = new Person("Jagadish Chakma",26);
Person* p2 = new Person("Jotis Moni Chakma",27);
*p1 = *p2;
```

```c++
Person* p1 = new Person("Jagadish Chakma", 26);
Person* p2 = new Person("Jotis Moni Chakma",27);
(*p1).name = (*p2).name;
```
# Content Index
- Introduction OOP
- Classes 
- Objects
- Members, outside mehtods, inside mehod
- Access Specifier
- Parameters
- Construction
- Encapsulation, get, set
- Inheritance, multilevel, multiple
- 
# What is OOP?
- OOP stands for Object-Oriented Programming.
- Procedural programming is about writing procedures or functions that performs operations on the data, while object-oriented programming is about creating objects that contain both data and objects.
- Object-oriented programming has several advantages over procedural programming.
	- OOP is faster and easier to execute.
	- OOP provides a clear structure for the programs.
	- OOP helps to keep the C++ code DRY "Don't Repeat Yourself", and makes the code easier to maintain, modify and debug.
	- OOP makes it possible to create full reusable applications with less code and shorter development time.

# What are Classes and Objects?
- Classes and Objects are the two main aspects of object-oriented programming.
- A class is a template for objects, and an object is an instance of class.
- When the individual objects are created, they inherit all the variables and functions from the class.
- ==The classes blueprint also called user defined data type==

---

# Why We Need Class and Object?
- Class and Object not only use for OOP. It's also use for ==grouping==.
- ==Grouping== means store multiple data in a sigle block.
- 




---

# Classes and Objects
- C++ is an object-oriented programming language.
- Everything in C++ is associated with classes and object, along with its attributes and methods. For example: in real life, a car is an **object**. The cas has **attributes**, such as weight and color, and **methods**, such as drive and brake.
- Attributes and methods are basically variables and functions that belongs to the class. These are often referred to as "class members".
- A class is user-defined data type that we can use in our program, and it works as an object constructor, or a "blueprint" for creating objects.
- attributes = variables/members
- mehods = functions/members
- class = bluprint/template/user-defined data type
- ==classes name always should declare with Capitalization==;
- ==In class blueprint not have initial data==.
- ==When create object then assign data in class blueprint==
- ==class=data_type and object=variable_name==.
- ==classs also create a memory address and her under took memory address members list==.
- 


# Create a Class
To create a class, use the ==class== keyword.
==Create a class like blueprint or template==.
==class== = ==data_type==.
###### syntax
```c++
class MyClass{   // the class
	public:      // access specifier
	int age;     // attribute
	string my_name; // attribute
}; // semicolon
```

###### explain
- The ==class== keyword used to create a class called ==MyClass==.
- The ==public== keyword is an **access specifier**, which specifies that members (attributes and methods) of the class are accessible from outside the class.
- Inside the class, there is an integer variable ==age== and a string variable ==my_name==. When variables are declared within a class, they are called attribute.
- At last, end the class definition with a semicolon ; .


# Create an Object
- In C++, an object is created from a class. 
- To create an object of ==MyClass==, specify the class name, followed by the object name.
- ==Create  a object like varible declare==.
- ==object=== = ==variable_name==.
###### syntax
```c++
int main(){
	data_type variable_name // syntax
	MyClass jagadish; // create an object
	return 0;
}
```


# Access  To The Class Members
- To access the class members or attributes or mehods, use the dot (.) syntax on the object.
###### syntax
```c++
int main(){
	MyClass jagadish; // create an object
	jagadish.age = 26; // access members
	jagadish.my_name = "Jagadish Chakma"; // access members
	return 0;
}
```


# Create Multiple Objects
You can create multiple objects of one class:
###### syntax
```c++
int main(){
	MyClass jagadish,sushil,jotis_moni; // create multiple objects
	return 0;
}
```



---


# Class Methods
- Methods are functinos that belongs to the class.
- There are two ways to define functions that belongs to a class:
	- Inside class definition
	- Outside class definition
# Inside Class Definition
```c++
class MyClass{
	public:
	int age;
	string my_name;
	void full_name(){ // inside definition
		// code to be executed
	}
}
```

# Outside Class Definition
```c++
class MyClass{
	public:
	int age;
	string my_name;
	void full_name(); // outside definition
};

void MyClass::full_name(){ 
	// code to be executed;
}
```


# Parameters
```c++
class MyClass{
	public:
	int age;
	stirng my_name;
	void full_name(string my_full_name){ // define parameters
		cout << my_full_name << endl;
	}
}

int main(){
	MyClass jagadish;
	jagadish.full_name("Jagaddish Chakma"); // add arguments
	return 0;
}
```



---


#  Constructors
- A constructor in C++ is a **special method** that is automatically called when an object of a class is created.
- To create a constructor, use the same name as the class name, followed by parantheses ==()==;
- Constructor is a function.
- Constructor does not have a return value.
- Constructor function use for initial setup value;
- When class is laoding first of all constructin function is executed.
- Constructor automatically called when object create.
- Constructor can receive parameter.
- Constructor does not have return type.
# Create Constructor
```c++
class MyClass{
	public:
	MyClass(){ // this is construction function
		// conde to be executed;
	}
}
```


# Constructor Parameters
- Constructors can also take parameters (just like reqular functions), which can be for setting initial values for attributes.
```c++
class MyClass{
	public:
	int age;
	string my_name;
	Myclass(int age, string my_name){
		age = age;
		my_name = my_name;
		cout << age << endl << my_name << endl;
	}
}

int main(){
	MyClass jaadish(23,"Jagadish Chakma");
	return 0;
}
```


# this keyword
- ==this== is a pointer that refers outside class.
- arrow sign(=>)
```c++
(*this).member
this->member
```


---
# Return object from function and why we need dynamic object?
- return object return copy of object.
- return object address and data will be lost.see
- create dynamic object for this solution
```c++
Person* jaga = new Person("Jagadish Chakma", 26)
```
- delete dynamic object
```c++
Person* jaga = new Person("Jagadish Chakma",26);
delete jaga;
```

---

# Access Specifiers
- Access specifiers define how the members (attributes and methods) of a class can be accessed.
- In C++, there are three access specifiers:
	- ==public== - members are accessible from outside the class.
	- ==private== - members cannot be accessed (or viewed) from outside the class.
	- ==protected==  - members cannot be accessed from outside the class, however, they can be accessed in inherited classes.

- By default, all members of a class are ==private== if you don't specify an access specifier.

###### examples
```c++
class MyClass{
	public:
	int age; // public
	private: 
	string my_name; // private
}
```

###### examples
```c++
class MyClass{
	int age; // auto private
	string my_name; // auto private
}
```


---

# Encapsulation
The meaning of **Encapsulation**, is to make sure that "sensitive" data is hidden from users. To achive this, you must declare class variables/attributes as ==private== (cannot be accessed from outside the class). If you want others to read or modify the value of a private member, you can provide public **get** and **set** methods.

# Access Private Members
To access a private members, use public "get" and "set" methods:
```c++
class MyClass{
	private:
	int age;
	string my_name;
	public:
	void setValue(int p1, int p2){
		age = p1;
		my_name = p2;
	};
	void getValue(){
		cout << age << endl << my_name << endl;
	}
}
```


# Why Encapsulation?
- It is considered good practice to declare your class attributes as private (as often as you can). Encapsulation ensures better control of your data, because you (or others) can change one part of the code without affecting other parts.
- Increased security of data.



#  What is Encapsulation?
Encapsulation means sensitive class members ensure as ==private== , and modify using ==get== and ==set== system.


---

# Inheritance 
- In C++, it is possible to inherit attributes and methods from one class to another. 
- We group the "inheritance concept" into two categories :
	- derived class/child class - the class that inherits from another class.
	- base class/parent class - the class being inherited from.
- To inherit from a class, use the ==:== symbol.

###### example
```c++
class MyClass1{ // base class
	public:
	string country_name = "Bangladesh";
};

class MyClass2: public MyClass1{ // child class
	public:
	string city = "Rangamati";
};

int main(){
	MyClass2 country;
	cout << country.country_name << endl << country.city << endl;
	return 0;
}
```


# Multilevel Inheritance
- A class can also be derived from one class, which is already derived from another class.
###### example
```c++
class MyClass1{ // base class
	public:
	string country_name = "Bangladesh";
};

class MyClass2: public MyClass1{ // child class
	public:
	string city = "Rangamati";
};
class MyClass3: public MyClass2{
	public:
	int zip_code = 4500;
};

int main(){
	MyClass3 country;
	cout << country.country_name << endl << country.city << endl <<       country.zip_code;
	return 0;
}
```


# Multiple Inheritance
- A Class can also be derived from more than one base class, using a comma-separated list.

###### example
```c++
class MyClass4: public MyClass3, public MyClass2, public MyClass1{

}
```


# Why And When To Use "Inheritance"?
- It is useful for code reusability: reuse attributes and methods of an existing class when you create a new class.


---



