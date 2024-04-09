# Capacity
- s.==size()== => returns the size of the string.
- s.==max_size()== => returns the maximum size that string can hold.
- s.==capacity()== => returns current available capacity of the string.
- s.==clear()== => clear the string.
- s.==empty()== => return true/false if the string is empty.
- s.==resize()== => change the size of the string.
# Element Access
- ==s[i]== => access the nth index of the string.
- s.==at(i)== => access the nth index of the string.
- s.==back()== => access the last element of the string.
- s.==front()== => access the first element of the string.

# Modifiers
- **s+=** => append anotehr string.
- **s.append()** => append another string.
- **s.push_back()** => add character to the last of the string.
- **s.pop_back()** => remove the last character of the string.
- **s=** => assign string.
- **s.assign()** => assign string.
- **s.erase(start,end)** => erase character from the string.
- **s.replace(start,how,add)** => replace a portion of the string.
- **s.insert(start,add)** => insert a portion to a specific position.
- s[20] = can't increase size of memory in this way.

# Iterators(pointer)
- s.==begin()== => pointer to the first element.
- s.==end()== => pointer to the next element after the last element of the string.
```c++
string::iterator it;
for(it = s.begin(); it < s.end(); it++){
	cout << *it << endl;
}
```
