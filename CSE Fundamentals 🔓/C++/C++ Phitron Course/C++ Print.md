# Phitron
- C used ==stdio== header file for input and output. On the other hand C++ used ==iostream== for input and output.
```c++
#inlcude <iostream>
```
- C used ==main()== funtion. Also C++ used ==main()== function.
- C used ==printf()== function for output. C++ used  ==cout== for output.
```c++
#include <iostream>
int main(){
	std::cout << "Hello C++";
	return 0;
}
```
- C++ extra use named ==namespace== . It is a group that here can store multitple things.
- ==cout== is not function. It is like command.
- C variable print using ==printf("%d",a)== vs C++ variable printf. C++ does not have formate spacifier.
```c++
#include <iostream>
int main(){
	int a = 12;
	std::cout << a;
	return 0;
}
```
- C uses for new line =="\n"== vs c++ uses for new line ==endl== or =="\n"== .
```c++
#include <iostream>
int main(){
	int a = 12;
	std::cout << a << std::endl << " Good Evening!";
	return 0;
}
```
- C multiple print vs C++ multiple print.
```c++
#include <iostream>
int main(){
	int a = 12;
	int b = 432;
	string name = "Jagadish Chakma";
	std::cout << a << endl << b << endl << name;
	return 0;
}
```

# C++ Output(print)
The ==cout== object, together with the ==<<== operator, is used to output values/print text.
You can add as many ==cout== objects as you want.
It does not insert a new line at the end of the output.

### Pronounced
==cout== is pronounced "see-out".

## Initital Setup

```c++
#include <iostream>
using namespace std;
int main(){
//code here
return 0;
}
```


### Output Text

```c++
cout << "Output text"
```


### Output Variable

```c++
int a = 23;
cout << a;
```


### Output Text With Variable

```c++
int a = 324;
int b = 34;
cout << a << " " << b;
```


