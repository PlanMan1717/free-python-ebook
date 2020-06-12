# This is for people who are familiar with C++

## Refresher

As a C++ programmer, you are already with the concept of data types. Every time you create a variable you must write out something like:

 
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
name = input("What is your name? ")
print("Oh, Hello " + name)
```

Let's break that one down.
- `name` is a string because `input` will **always** return a string.
- `input` takes an argument of (almost) any type to be the prompt. This is accomplished without any overloads.
- `print` will print the text specified to the terminal. More on this soon.
- When using a `+` operator to add strings, it is called "concatenation". It puts the second string on the end of the first without changing whitespace.

We needed no sort of libraries to perform that. The functions are called "builtins".

### More on data types

- Literally everything is a variable.
	- `print` can be called without parens, it returns `<built-in function print>`
	- Classes are vari
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTY3MTAxNjc3Nl19
-->