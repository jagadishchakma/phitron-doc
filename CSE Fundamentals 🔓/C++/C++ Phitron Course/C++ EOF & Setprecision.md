# Phitron
- EOF in C: ==EOF== use for infinity input in C.
```c
#inlcude <stdio.h>
int main(){
	int a,b;
	while(scanf("%d %d",&a,&b) != EOF){
		printf("%d %d", a, b);
	}
	return 0;
}
```
- EOF in C++: ==EOF== not necessary for infinity in C++.
```c++
#include <iostream>
using namespace std;
int main(){
	int a,b;
	while(cin>>a>>b){
		cout << a << end << b << endl;
	}
	return 0;
}
```
- C uses ==".2%lf"== vs C++ uses==setprecision()==  for how many digits accept after decimal . With declare ==iomanip== package.
```c++
double a = 23.3232323;
cout << fixed << setprecision(2) << a << endl;
```
