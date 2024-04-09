## Create
- using object literal:
	- var obj = {};
- using constructor function:
	- function Person(){}
	- var obj = new Person();
- using built-in object:
	- var obj = Object();
	- var obj = new Object();
- usng es6 class syntax:
	- class Person{}
	- var obj = new Person();
- using Object.create method:
	- var obj = Object.create({});
- using Object.assign:
	- var obj = Object.assign({},{});
## Behind The Scene:
- Why object is a data type?
	- Object is a custom data type behind the scene working in c++.
	- Object literal behind the scene convert into the c++ class object.
	- In class object c++ create some ==built in property or method using some header files or custom== for manipulate javascript object.
		- ==Properties==
			- constructor
			- prototype
		- ==Methods==
			- ==Object.assign(target,source1,source2...);== copy reference, return new obj, change original
			- ==Object.assign({},source1,source2..);== clone, return new obj, not change original
			- ==Object.create(single or empty obj);== clone, return new obj, not change original,hide original properties
			- ==Object.defineProperties(obj,{{pro1,pro2..}});== define multiple properties for obj object. or modify existing properties with security.
				```js
				pro1:{
					value: "value",
					writable: true // will be change using assginment
					enumerable: true // will be listed during object   enumeration
					configurable: true // can be deleted and proeprty attributes can be modified
				}
				```
			- ==Object.defineProperty(obj,'propertyName',{newSecurity});== define single property for obj object, or modify existing property with security.
			- ==Object.entries(obj);== return an array of [key,value] pairs. iterate - for(let [key,value] of entries);
			- ==Object.freeze(obj);== no return, not mutable obj object after that
			- ==Object.fromEntries(obj);== return object, create obj from key values paris.
			- ==Object.getOwnPropertyDescriptor(obj,'prop');== return the single property security info with value.
			- ==Objec.getOwnPropertyDescriptors(obj);== return an object secrity description info with value.
			- ==Object.getOwnPropertyNames(obj);== or ==Object.keys(obj);== return an array of object property names.
			- ==Object.values(obj);== return an object values.
			- ==Object.seal(obj);== no return, cant' add,delete,property and security only change propery value.
			- ==obj.hasOwnProperty(propertyname);== return boolean is or not property has.
	- Behind the scene javascript object always store in ==heap== memory in c++ code.
	- That's why javascript object are also called reference data type.
	- 