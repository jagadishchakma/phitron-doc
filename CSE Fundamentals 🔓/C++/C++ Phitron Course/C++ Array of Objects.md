# Phitron
- ==Array of Objects== like general array.
- But this array holding only objects.
```c++
Person a[n];
```
- Dynamic array of objects.
```c++
Person* a = new Person[n];
```
- array of objects min
```c++
Person a = Person[n];
Person mn = a[0];
for(int i = 0; i < n; i++){
	if(a[i].marks < mn.makrs){
		mn=a[i];
	}
}
```
- array of objects mx
```c++
Person a = Person[n];
Person mx = a[0];
for(int i = 0; i < n; i++){
	if(a[i].marks > mn.marks){
		mn = a[i];
	}
}
```
