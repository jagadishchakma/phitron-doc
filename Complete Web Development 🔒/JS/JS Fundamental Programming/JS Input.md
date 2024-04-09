- It's commonly take input from browser.
- In terminal can take input:
```js
const readline = require("readline");
const rl = readline.createInterface({
	input: porcess.stdin,
	output: process.stdout,
});

rl.question("Input",(input)=>{
	console.log(input);
});
```
- Genrally when working,practice with javascript, manually take the value