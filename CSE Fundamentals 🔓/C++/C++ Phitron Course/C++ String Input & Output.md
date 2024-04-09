- String initialized;
```c++
char s[] = "String Inut & Output";
cout << s;
```
- String input with space  C ==fgets()== vs C++ ==cin.getline()== 
```c++
char name[100];
cin.getline(name,100);
cout << name;
```
- String length with inlcude ==string.h== 
```c++
#include <iostream>
#include <string.h>
using namesapce std;
int main(){
	char name[100];
	cin.getline(name,100);
	cout << strlen(name) << endl;
	return 0;
}
```
- Remove enter input using ==getchar()== when getting string input using ==getline==
```c++
int age;
char name[100];
cin >> age;
getchar();
cin.getline(name,100)
```
