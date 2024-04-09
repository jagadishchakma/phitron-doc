# Phitron
- Discussion about STL.
- Discussion about Vactor.
- Initialized a vactor?
- Vactor constructor.
- Vactor built-in function, Capacity, Modifiers.
- Vactor access, iterator.
- Take input in vactor.
- String vactor.
### Discussion about STL
- STL full meaning of Standard Template Library.
- STL is a c++ library,where included data structure implemented built in function. Data structure implentation is long process, so that using STL we just use pre-defined data structure functions.But remember that before implement STL must be know how to work data structure.
- The STL is a powerfull set of C++ template classes to provide generaL-purpose classes and functions with templates that implement many popular and commonly used algorithms and data structures like vactors, list, queues, and stacks.
- It consists of several component, including ==algorithms,containers,functions and iterators== . The STL allows you to use generic programming techniques, making your code more reusable and efficient.
### Discussion about Vactor
- Vactor is one of the containers provided by STL.
- Using vactor we can manipulate easily dynamic array.
- In C++, a vactor is a dynamic array implementation provided by the STL. It is a sequence container that is similar to an array but can dynamically resize itself. Vectors are part of the C++ Standard Template Library(STL).
- Key characteristics of vectors include constant-time random access to elements, dynamic resizing, automatic memory management, and contiguous storage.

### Initialized a Vector.
There are several ways to initialized a vactor in C++. Here are some common methods:
- Empty Initialization:
```c++
vector<data_type> vector_name;
vector<int> myVector; // Creates an empty vector of integers
```
- Initialization with size:
```c++
vector<data_type> vector_name(size);
vector<int> myVector(5); // Creates a vector with 5 default-initialized integers (0 for int)
```
- Initialization with Size and Initial Value:
```c++
vector<data_type> vector_name(size,value); // Creates a vector with size and value;
vector<int> myVector(5,10);
```
- Initialization with existing vector:
```c++
vector<data_type> vector_name1(size,value);
vector<data_type> vector_name2(vector_name1); // Creates a vector with existing vector.
vector<int> myVector1(5,1);
vector<int> myVector2(myVector1);
```
- Initialization using an existing array:
```c++
int arr[] = {1,2,3,4,5};
vector<int> myVector(arr,arr+sizeof(arr)); // Creates a vector with existing array
```
- Initialization Using an Initializar List (C++ 11 or later):
```c++
vector<int> myVector = {1,2,3,4,5};
```
- Range initialization (C++ 11 or later):
```c++
vector<int> myVector{1,2,3,4,5};
```
- Copy Initialization from Another Vector:
```c++
vector<int> myVector1 = {1,2,3,4,5};
vector<int> myVector2 = myVector1;
```
### Vector Built-In Function
###### Constructor:
| Name | Details | Time Complexity |
| ------ | --- | --- |
|vector\<type\>v;|Constructs a vector element with 0 elements|O(1)|
|vector\<type\> v(N)|Construct a vector with N elements and the value will be V.|O(N)|
|vector\<type\> v(N,V)|Construct a vector with N elements and the value will be V.|O(N)|
|vector\<type\> v(v2)|Construct a vector by copying another vector v2.|O(N)|
|vector\<type\> v(A,A+N)|Construct a vector by copying all elements from an array A of size N.|O(N)|
##### Capacity
| Name | Details | Time Complexity |
| ----- | ------ | ------- |
|v.size() | Returns the size of the vector | O(1) |
|v.max_size() | Returns the maximum size that the vector can hold | O(1) |
|v.capacity() | Returns the current available capacity of the vector. | O(1) |
|v.clear() | Clears the vector elements. Do not delete the memory, only clear the value. | O(1) |
|v.empty() | Return true/false if the vector is empty or not. | O(1) |
|v.resize() | Change the size of the vector. | O(k); where k is the difference between new size and current size. |
### Modifiers
| Name | Details | Time Complexity |
| ----- |----| ----- |
|v=,v.assign()|Assign another vector.|O(N) if sizes are different, O(1) otherwise|
|v.push_back()|Add an element to the end|O(1)|
|v.pop_back()|Remove the last element|O(1)|
|v.insert(a.begin()+x,b.begin(),b.end())|Insert element at a specifc position using pointer| O(N+K); where k is the difference between new size and current size|
|v.erase()|Delete elements from a specific pointer position | O(N+K); where k is the number of elements to be deleted.|
|replace(v.begin(),v.end(),remove_value,add_value)|Replace all the value with repalce_value. Not under a vector. | O(N) |
|find(v.begin(),v.end(),V) | Find the value V. Not under a vector. | O(N) |

### Element Access:
|Name|Details|Time Complexity|
|------|-------|-----|
|v[i]|Access to ith element.|O(1)|
|v.at(i)|Access the ith element.|O(1)|
|v.back()| Access the last element|O(1)|
|v.front()|Access the first element|O(1)|

### Iterators
|Name|Details|Time Complexity|
|------|------|-----|
|v.begin()|Pointer to the first element | O(1) |
|v.end()| Pointer to the last element |O(1)|
