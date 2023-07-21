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

**ex 1**
```
name = input("Please enter your name: ")
print(f"Hello {name}")
```
```
python example_1.py
Please enter your name: Miyuki
Hello Miyuki
```

To call a function you need to the following 3 things: 
1. The name of the function.
2. The parameters that the function accepts.
3. What the function does.

Look in the online documentation to find the 3 important pieces of information.

[Input - Reference](https://docs.python.org/3/library/functions.html#input)
 
> input(prompt)
>
> Write the *prompt* parameter to the terminal window, then read a line of user input from the window, convert the input to a string, and return the input as a string.

From this description we learn the following:
- The name of the function is input.
- The function accepts one parameter, which is named *prompt*.
- The function writes the prompt to a terminal window and then reads user input from the terminal and returns that input to the calling function.

> A *parameter* is a piece of data that a function needs in order to complete its task.

In the online reference for the [Input Function](https://docs.python.org/3/library/functions.html#input), we see that the input function has one parameter named *prompt*.

> An *argument* is the value that is passed through a parameter into a function.

Parameters are listed in a function's documentation, and arguments are listed in a call to a function.

#### Write code that calls a function.
1. Type a new variable name and use the assignment operator (=) to assign a value to the variable.
2. Type the name of the function followed by a set of parentheses.
3. Between the parentheses, type arguments that the computer will pass into the function through its parameters.

The following example calls the built-in input function and passes the string "Please enter your name: " as the argument for the *prompt* parameter. 

```
name = input("Please enter your name: ")
```

### Optional Arguments

Some arguments are optional when you call a function or a method.

> round(number, ndigits)
>
> Return *number* rounded to *ndigits* precision after the decimal point. If *ndigits* is omitted or is None, round return the nearest integer to *number*.

**ex 2**
```
n = float(input("Please enter a number: "))
r = round(n, 2)
print(r)
```
```
python example_2.py
Please enter a number: 95.716
95.72
```

**ex 3**
```
n = float(input("Please enter a number: "))
r = round(n)
print(r)
```
```
python example_3.py
Please enter a number: 95.716
96
```

### Named Arguments

For some optional arguments we need to pass a *named argument*. A named argument is an argument that is preceded by the name of its matching parameter. 

print function
> print(*objects, sep=" ", end="\n", file=sys.stdout, flush=False)
>
> Print objects to text stream *file*, separated by *sep* and followed by *end*. *sep*, *end*, *file* and *flush*, if present, must be given as named arguments. 
