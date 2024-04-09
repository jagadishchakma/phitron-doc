## Access Prototype
- Number.prototype
- String.prototype
- Object.prototype
- Array.prototype
- Boolean.prototype
- Function.prototype
- funciton_name.prototype
- Date.prototype
- Symbol.prototype
- Error.prototype
- RegExp.prototype
## Behind The Scene
- prototype is a property of functions object.
- Every ==constructor== functions have a property object of ==prototype== .
- Above all are ==master object with global object with constructor function==.
- JS all data type has a ==master== object. And this master object has a property called ==prototype== . This prototype is a object. and hold many ==properties== and ==methods==
- So , prototype is a property of master object and prototype itself a object.
```js
class Array{
	constructor(...p){
		this = p;
	}
	prototype = {
		map: () => {},
		forEach: () => {},
		reduce: () => {}
	}
}
const arr = [1,2,3,4] like const arr = new Array(1,2,3,4);
```
