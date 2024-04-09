# C
- ### construct
# C++
- ### class
	- ###### Key Points
		- ==User defined data type.==
		- For storing multiple data type in a group.
	- ........Create..........
```c++
	class MyClass{
		public:
		int age; //property
		string name; // property
		string study; // property
	}
```
- 
	- ..........Constructor........
		- automatically called when function called;
```c++
class MyClass{
	public:
	int age; // property
	string name; // property
	string study; // property
	MyClass(){ // constructor method
	
	};
}
```
- 
	- ..........this........
		- ==this== is a pointer of self object;
```c++
class MyClass{
	public:
	int age;
	string name;
	string study;
	MyClass(int age, string name, string study){
		this->age = age;// (*this).age = age;
		this->name = name;//(*this).name = age;
		this->study = study;//(*this).study = age;
	}
}
```

- ### Object
	- ###### Key Points
		- It's a instance of class.
	- .........Create...........
		- ==MyClass obj== // static object
		- ==MyClass obje()== // static object with Constructor
		- ==MyClass obj = new MyClass()== // dynamic  object with constructor
	- .........Insert...........
		- obj.age = value;
		- obj.name = value;
		- obj.study = value;
	- .........delete...........
		- ==delete obj==
		
# JS
- ### class
	- ###### Key Points
		- ==User defined data type.==
		- For storing multiple data type in a group.
	- ........Create..........
```js
	class MyClass{
		
		age; //property
		name; // property
		study; // property
	}
```
- 
	- ..........Constructor........
		- automatically called when function called;
```js
class MyClass{
	constructor(age,name,study){
		console.log(age,name,study);
	}
}
```
- 
	- ..........this........
		- ==this== is a pointer of self object;
```js
class MyClass{
	constructor(age,name,study){
		this.age = age;
		this.name = name;
		this.study = study;
	}
}
```

- ### Object
	- ###### Key Points
		- It's a instance of class.
	- .........Create...........
		- ==const obj = new MyClass()== // dynamic  object with constructor
	- .........Insert...........
		- obj.age = value;
		- obj.name = value;
		- obj.study = value;
	- .......delete..........
		- ==delete obj.prope===
		

