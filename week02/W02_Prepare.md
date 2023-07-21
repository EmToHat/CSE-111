# W02 Prepare: Calling Functions


### What is a Function?

> A *function* is a group of statements (computer commands) that together perform one task. 

Python has 4 types of functions: 
1. Built-in functions
2. Standard library functions
3. Third-party functions
4. User-defined functions.

### Built-in Functions

Python includes many *built-in functions* such as:
- input, int, float, str, len, range, abs, round, list, dict, open, print

These are called built-in functions because nothing needs to be imported to be used. These functions are a built-in part of the Python language.
[Built-in Functions - Reference](https://docs.python.org/3/library/functions.html)

### How to Call a Function

A function is used when it is *called* / *invoked*. 

> To *call* or *invoke* a function means to write code that causes the computer to execute the code that is inside that function.

Regardless of the function type (built-in, standard, third-party, user-defined), a function is called by writing its name followed by a set of parentheses.

```
name = input("Please enter your name: ")
print(f"Hello {name}")
```

```
python example_1.py
Please enter your name: Miyuki
Hello Miyuki
```
