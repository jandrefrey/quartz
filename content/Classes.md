---
title: "Classes"
---
We can access the properties of a class by creating an instance of it.
An object is an instance of a class. (memory only allocated when object/instance is created)

The point of the class is to hide all unnecessary data and functions to the "outside world". Only the required input and output of the class is visible.
In C++, there are three access specifiers:

- `public` - members are accessible from outside the class
- `private` - members cannot be accessed (or viewed) from outside the class
- `protected` - members cannot be accessed from outside the class, however, they can be accessed in inherited classes. 

The meaning of **Encapsulation**, is to make sure that "sensitive" data is hidden from users. To achieve this, you must declare class variables/attributes as `private` (cannot be accessed from outside the class). If you want others to read or modify the value of a private member, you can provide public **get** and **set** methods.

Properties can be inherited from one class to another.
- **derived class** (child) - the class that inherits from another class
- **base class** (parent) - the class being inherited from
To inherit from a class, use the `:` symbol.