# Phitron
- Strings is a class an object.
- You can access strings member like general object access.
- String declare way:
```c++
string name = "Jagadish Chakma"; //one way
string name("Jagadish Chakma"); //two way
string name("Jagadish Chakma",6); //third way
string name = "Jagadish Chakma"; // fourth way
string fullName(name,4); // fourth way
```
- Sort string using ==sort()== functions.
```c++
string name = "Jagadish Chakma";
sort(name.begin(),name.end());
cout << name;
```
- String in for loop
```c++
string name = "Jagadish Chakma";
for(char c:name){
	cout << c << endl;
}
```

# Introduction
- Strings are used for storing text.
- A ==string== variable contains a collection of characters surrounded by ==double== quotes.
- Create a variable of type ==string== and assign it a value.
- To use strings, you must include an additional header file in the source code, the ==string>== library.
- An string in c++ is actually an object, which contain functions that can perform certain operations on strings.
```c++
string name = "Jagadish Chakma";
```
# String Concatenation
- C++ uses the + operator for both addition and concatenation.
- Numbers are added.Strings are concatenation.
- The ==+== operator can be used between strings to add them together to make a new string. 
```c++
string first_name = "Jagadish";
string last_name = "Chakma";
string full_name = first_name + last_name;
```
- You can also concatenate strings with the ==apend()== function
```c++
string first_name = "Jagadish";
string last_name = "Chakma";
string full_name = frist_name.append(last_name);
```
# String Length
- To get the length of a string, use the ==length()== or ==size()== function.
```c++
string full_name == "Jagadish Chakma";
int length = full_name.length();
int length2 = full_name.size();
```
# String Character Access
- You can access the characters in a string by referring to its index number inside squre bracket [].
```c++
string full_name = "Jagadish Chakma";
cout << full_name[3];
```
- String indexes start with 0.
- To change the value of a specific character in a string, refer to the index number, and use single quotes:
```c++
stirng full_name = "Jagadish Chakma";
full_name[4] = 'k';
cout << full_name << endl;
```
# String Input
- It is possible to use the extraction operator >> on cin to store a single word word string without spcae.
```c++
string full_name;
cin >> full_name;
```
- However, ==cin== consider a space (whitespace, tabs, etc) as a terminating character, which means that it can only stroe a signle word(even if you type many words);
- That's why, when working with strings, we often use the ==getline()== function to read a line of text.
```c++
string full_name;
getline(cin, full_name);
```

# Sort String Using sort() Function
```c++
string full_name = "Jagadish Chakma";
sort(full_name.begin(), full_name.end());
```
# Ranged Based For Loop In String.
- If you need index go to for loop.
- If you need only value go to ranged based loop.
```c++
string full_name = "Jagadish Chakma";
for(char c:full_name){
	cout << full_name << endl;
}
```

# String Input With Space
- Take input with space using ==getline(cin,s)==
```c++
string name;
getline(cin,name);
```
- Avoid enter using ==cin.ignore()== or ==getchar()==
```c++
	int a;
	string name;
	cin >> a;
	cin.ignore();
	getline(cin,name);
```
# String Word Manipulate
- manipulate using ==stringstream== keyword
```c++
string name = "My name is Jagadish Chakma";
stringstream wrodstream;
name >> wordstream;
string word;
while(wordstream >> word){
	cout >> word;
}
```
