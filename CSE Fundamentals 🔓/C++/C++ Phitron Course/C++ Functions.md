
# Introduction
- A function is a block of code which only runs when it is called.
- You can pass data, known as parameter, into a function.
- Function are used to performs certain actions, and they are important for reusing code. Define the code once, and use it many times.

# Create a Function
- C++ provides some pre-defined functions, such as ==main()== , which is used to execute code.
- But you can also create your own functions to perform certain actions.
###### syntax
```c++
void my_function(){
	// code to be executed
}
```
- ==void== return type.
- ==my_function== name of function.
- ==body== // coe to be executed.
- ==declaration== return type, function name, parameters
- ==definition== body

***==Note:==If a user defined function declared after the ==main()== function, an error will occur.***

###### Example
```c++
void sum(){
	int a = 3, b= 4;
	int result = a + b;
	cout << result << endl;
}
int main(){
	sum();
}
```


# Call a Function
- Declared function are not executed immediately. When it is called then it is executed.
###### syntax
```c++
my_function();
```
###### example
```c++
int main(){
	my_function()// function called inside main function
	return 0;
}
```


----
# Parameters
- Information can be passed to functions as parameter.
- Parameters act as variable inside the function.
- You can add as many parameters as you want. Just separate then with comma (,).
###### syntax
```c++
void my_function(type p1, type p2, type p3){
	// code_to_be_executed
}
```
###### example
```c++
void my_function(int a, int b, stirng name){
	cout << a+b << endl;
	cout << name << endl;
}
```


# Arguments
- When a parameter is passed to the function when it is caled, is called an argument.
###### syntax
```c++
int main(){
	int a=12,b=23;
	string name = "Jagadish Chakma";
	my_function(a,b,name); // a,b,name are arguments
	return 0
}
```


----

# Default Parameters
- You can also use a default parameter value, by using the equal sign = .
- If we call the function without an argument, it uses the default value.
- A parameter with a default value, is often known as an **optional parameter** .
###### syntax
```c++
void my_function(int a = 23);
```
###### example
```c++
void my_function(int a, int b = 34){
	cout << a + b << endl;
}
int main(){
	my_function(10);
	return 0;
}
```


---

# Return Values
- The ==void== keyword, used in the previous example, indicates that the function should not return a value. If you want the function to return a value, you can use a data type (such as ==int== ==string== etc) instead of ==void==, and use the ==return== keyword.
###### syntax
```c++
data_type function_name(){
	return value;
}
```
###### example
```c++
int my_function(int a, int b){
	return a+b;
}
int main(){
cout << my_function(12,23) << endl;
	return 0;
}
```
