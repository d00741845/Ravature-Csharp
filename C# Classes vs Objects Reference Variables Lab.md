# Classes vs Objects, and Reference Variables

In C#, it's important to understand the difference between a Class, an Object, and a Reference Variable.

A class is a template used to instantiate objects. It's also called a type when used with a reference variable. A class used to instantiate an object determines what states and behaviors an object will possess. A class used as the type for a reference variable determines what behaviors of an object can be invoked, and some any variables get initialized.

An object is an instance of a class in memory. In C#, you rarely interact with objects directly. Instead, you interact with them through their reference, which is the memory address used by the CLR to find a particular object.

A reference variable is a variable that stores the reference to an object in memory. Just like the type of a primitive variable determines the range of values that a primitive variable can store, the type of a reference variable determines what types of objects a reference variable can store a reference to. When a class is used as the type of a reference variable, that reference can only be used to invoke behaviors of the object that are declared in the class/type.

Example: 
```c#
Dog someVar = new Dog();
  1      2         3
```
1 = The class/type of the reference variable
2 = The name of the reference variable
3 = The instantiation of a new object using the new keyword to invoke the constructor

- The someVar reference variable does not contain a Dog object, it contains a reference that points to it in memory
- The Dog type means that someVar can only store a reference to an object that is an instance of the Dog class (directly or through inheritance)
- The Dog type means that someVar can only be used to invoke methods or access public variables present in the Dog class (whether defined in Dog or inherited from a superclass)
- The "new Dog()" expression creates an object, it is not the object itself. 
Understanding these concepts and their implications is key to properly understanding the C# language.

---

Created by:
Jesse Fore

service.awg@gmail.com

Updated:
22 February 2020

-_-
---
