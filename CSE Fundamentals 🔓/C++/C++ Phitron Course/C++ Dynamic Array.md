# Create Dynamic Array
```c++
new data_type[size];
```

#### Example
```c++
int *a = new int[5];
```

# Dynamic Array Return From Function
```c++
int *fun(){
	int *a = new int[5];
	return a;
}
int main(){
	int *a = fun();
	cout << a[0];
	return 0;
}
```

# Increase Size of Dynamic Array

#### Follow Steps In Raw
- create one
- create two then copy all one
- delete one
- create again one but size increase ==!important==
- copy two all into one
- delete two
- then extra add into one
#### Example
```c++
int *a = new int[3];
int *b = new int[3];
for(int i = 0; i < 3; i++){
	a[i] = i;
	b[i] = i;
}
delete[] a;
a = new int[5];
for(int i = 0; i < 3; i++){
	a[i] = b[i];
}
delete[] b;
a[3] = 23;
a[4] = 34;
for(int i = 0; i < 5; i++){
	cout << a[i] << endl;
}
```

# About Delete
- To delete using ==delete== keyword
- Static value not possible to delete only dynamic value;
- Variable delete = ==delete== _variable_name
- Array delete = ==delete[]== _variable_name
