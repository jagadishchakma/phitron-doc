- ###### Pass a pointer in a function:
```c++
void fun(int* b){

}
int a = 23;
int* b = &a;
fun(b);
```
- ###### Change Pointer Value Using Direference:
```c++
void fun(int* b){
	*b = 234;
}
```
- ###### Not Change Pass Variable Value:
```c++
void fun(int* b){
	b = NULL;
}
```
- ###### Change Pass Variable Value:
```c++
void fun(int* &b){
b = NULL
}
```