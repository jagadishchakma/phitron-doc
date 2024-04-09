# Create Dynamic Memory
```c++
data_type *name = new data_type
```
#### Explain
- ==new== keyword automatically create a heap memory and create space based on data typpe.
- And returns her memory space address. ==!importan==t
- If you want to memory address manipulating then need to pointer.
#### Example
```c++
int *a = new int;
*a = 10;
cout << *a;
```
#### Function Return For Static Memory
```c++
int *fun(){
	int a = 10;
	return &a;
}
int main(){
	int *a = fun();
	cout << a << endl;
	return 0;
}
```
#### Function Return For Dynamic Memory
```c++
int *fun(){
	int *a = new int;
	*a = 10;
	return a;
}
int main(){
	int *a = func();
	cout << a << endl;
	return 0;
}
```
