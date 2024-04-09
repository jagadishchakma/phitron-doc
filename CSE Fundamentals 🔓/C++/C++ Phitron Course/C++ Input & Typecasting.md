# Phitron
- Also needs ==iostream== package for input in C++;
- C++ use right angle >> brakcet for take input.
- C used ==scanf()== function for input vs C++ used ==cin== command for take input.
```c++
#include <iostream>
int main(){
	int a;
	std::cin >> a;
	std::cout << a;
	return 0;
}
```
- ==std== reduce repeated writing ==using namespace std== after the all header files.
```c++
#include <iostream>
using namespace std;
int main(){
	int a;
	int b;
	cin >> a >> b;
	cout << a << endl << b;
	return 0;
}
```
- namespace means a group.
- Get ASCII value in C ==printf("%d", letter)== vs  C++: In C++ use ==single quoatation== for declare character.
```c++
char lett = 'a';
int ascii = lett;
cout << ascii;
```
- Get ASCII value using ==typecasting== .
```c++
char lett = 'a';
cout << (int)(lett);
```

# Input
C++ is used ==cin== to get user input.
==cin== is a predefined variable that reads data from the keyboard with the extraction operator (>>).
#### Pronounced
==cin== is pronounced "see-in".

#### Initial Setup
```c++
#include <iostream>
using namespace std;
int main(){
//code here
return 0;
}
```

#### Input Data
```c++
int a;
char b;
float c;
long long int d;
double e;
cin >> a >> b >> c >> d >> e;
```


______
# Typecasting
Type casting in c++ allows you to convert a value from one data type to another.

#### Declare
```c++
(data_type_name)(varaible_name)
```

##### 1 word data type name
```c++
int hundred = 100;
cout << char(ten);
```
##### Multiple word data type name
```c++
int seventy_five = 75999999999999999999999999999;
cout << (long long int) (seventy_five) << ebdl;
```
