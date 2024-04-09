# Introduction
- Namespace provide the space where we can define or declare identifier variable, method, classes.
- Using namespace, you can define the space or context in which indentifiers are defined variable, method, classes. In essence, a namespace defines a scope.
# Advantage of Namespace to avoid name colision
- Example, you might be writing some code that has a function called xyz() and there is another library available which is also having same function xyz(). Now the compiler has no way of knowing which version of xyz() function you are referring to within your code.
- A namespace is designed to overcome this difficulty and is used as additional information to differentiate similar function, classes, variables etc. with the same name available in different libreries.
# Defining a Namesapce
- A namespace definition begins with the keyword namespace followed by the namespace name as follows:
```c++
namespace namespace_name
{
	// variable,method,class code declaration
}
using namespace namespace_name;
```


