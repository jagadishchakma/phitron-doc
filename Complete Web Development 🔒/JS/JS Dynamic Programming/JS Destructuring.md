# Uses
- Array Destructure
	- const \[one,two] = \[1,2,3,4];
	- const \[,,three,four] = \[1,2,3,4];
	- const \[,,\[three,four]] = \[1,2,\[3,4]];
- Object Destructure
	- const {age} = {fname: "Jagadish", lname: "Chakma", age: 23};
	- const {age: boyos} = {fname: "Jagadish", lname: "Chakma", age: 23};
	- const {more: {fullName}} = {fname: "Jagadish", lname: "Chakma", age: 23, more:{fullName: "Jagadish Chakma"}};
	- 