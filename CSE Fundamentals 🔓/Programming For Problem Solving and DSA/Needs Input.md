# C
- #include<stdio.h>
- scanf();
- scanf("%d",&name);
- scanf("%d %d %d",&a, &b, &c);
- fgets(input, sizeof(input), stdin);
- & = empersized = address of
# C++
- #include\<iostream\>
- using namesapce std;
- cin >> name;
- cin >>a >> b >> c;
- getline(cin,name);
- cin.getline(name,size);
# JS
- let userInput = prompt("Enter something");
- using readine module
```js
const readline = require("readline");

const rl = readline.createInterface({

input: process.stdin,

output: process.stdout

});

  
  

let a, b, c;

rl.question("Enter: ",(inputA)=>{

	a=inputA;

	rl.question("Enter: ",(inputB)=>{

		b=inputB;

		rl.question("Enter: ",(inputC)=>{

			c=inputC;

			rl.close();

		});

	});

});
```

