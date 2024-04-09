# Promise
- ## Key Points
	- The Promise object represents the eventual ==completion== (or ==failure==) of an asynchronous operation and its resulting value. A promise is in one of these states.
	- JS Promise is a built in global object of JavaScript Programming lanuage and it's a self programming.
	- JS Promise is a async behavior.
	- ..........create............
	- ==const promise = new Promise(callback(reovle(),rejected()))
	- ...........catch resolved..............
	- ==promise.then((data)=>console.log(data))
	- ...........catch error...............
	- ==promise.catch((err)=>console.log(err))==
	- ............async/await............
	- async/awit ==then/catch== next remove.
	- =="async/await"== is a special syntax to work with the promise in a more comfortable way.
	- It's surprisingly easy to understand and use.
	- The ==await== keyword can only be used inside an async function.
	- The ==await== keyword makes the function pause the execution and 
	- wait for a resovled promise before it contains.
```js
const callback = (resolved,rejected) => resolved("Yes");
async function myfunc(){
	const promise = await new Promise(callback);
	console.log(promise);
}
myfunc();
```
