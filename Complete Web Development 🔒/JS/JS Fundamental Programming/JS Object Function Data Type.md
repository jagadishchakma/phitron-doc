## Declare
- general function
	- function myfunc(){codeblocks here}
- arrow function
	- const myfunc = () => {codeblocks here}
## Behind The Scene
- Behind the scene function why working as like Object:
	- Behind the scene function converted into the object in JS engine or c++ code.
	- After convereted object threads some properties and methods:
		- Properties:
			- myfunc.name
			- myfunc.length
			- arguments
		- Methods:
			- ==myfunc.call(obj,p1,p2..);== function call using call method for some advantage.
			- ==myfunc.apply(obj,[p1,p2]);== function call using apply method for some advantage.
			- ==myfunc.bind(obj,p1,p2..);== function return using bind method for some advantage.
		