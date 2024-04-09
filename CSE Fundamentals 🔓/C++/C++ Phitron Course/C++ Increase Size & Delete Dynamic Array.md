# Phitron
- To delete dynamic array:
```c++
delete[] arr;
```

```c++
#include <bits/stdc++>
using namespace std;
int* myfun(){
	int* a = new int[5]{1,2,3,4,5};
	return a;
}
int main(){
	int* a = myfun();
	cout << a[3];
	delete[] a;
	cout << a[2];
	return 0;
}
```
- To delete dynamic variable:
```c++
delete arr;
```

```c++
#include <bits/stdc++>
using namespace std;
void myfun(int* age){
	*age = 56;
}
int main(){
	int* age = new int;
	*age = 34;
	cout << *age << endl;
	myfun(age);
	cout << *age << endl;
	return 0;
	delete age;
	cout << *age << endl;
}
```

- Increase size of Array:
```c++
int* a = new int[3];
int* b = new int[3];
delete[] a;
a = new int[5];
// copy b element into a using loop
delete[] b;
// add more element into a array
```

