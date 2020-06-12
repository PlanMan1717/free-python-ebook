# This is for people who are familiar with C++

## Refresher

As a C++ programmer, you are already with the concept of datatypes. Every time you create a variable you must something like:

 
```c++
int score;
double health =  100.0;
char[] name;
```

Having a system like that does have its advantages, as you will learn. But, for now, simply understand that in Python, you don't need a datatype; it's implicit!

Now, the C++ code above will be rewritten in Python;

```python
score =  int()
health =  100
name =  ""

```

A few things to note:

1. You can't define an empty variable. That is why `score` was given the constructor `int()`. It could have been defined with `0` or the special variable `None`, all to the same effect.
2. Python is dynamically typed. A variable can be defined as a string, but then changed to an `float`.
3. The types don't have the same names!

C++ name | Python name
---------|---
`int`    | `int`
`double` | `float`
`float`  | `float`
`char`   | `chr`
`char[]` | `str`

Example:

```c++
#include<iostream>
int  main() {
char[] name;
std::cout <<  "What is your name? ";
std::cin >> name;
std::cout <<  "\n"  <<  "Oh, Hello "  << name << std::endl;

return  0;

}

```

  

Becomes:

  

```python
<!--stackedit_data:
eyJoaXN0b3J5IjpbMzgyODczNzQ2XX0=
-->