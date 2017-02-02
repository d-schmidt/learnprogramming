---
layout: default
title: "Calculator: The Basic Building Blocks"
categories: tutorials
---

# {{ page.title }}
{% include image.html url="/assets/images/LEGO_10696.jpg" description="Model 10696, ©The LEGO Group" %}
To teach you the very basics we are building something similar beautiful: a calculator

Hang in, this will only take a few hours.

Before you start typing, sit back for a moment and think about, what you need to add two numbers.

Now open the editor of you choice, create a new file and save it as `calculator.py`. Don't close the editor.  
Try to run it using the build in run or open a console, [cd][l7] to your file and type in `python calculator.py`.

```
i:\git\learnprogramming\examples>python calculator.py

i:\git\learnprogramming\examples>
```

Nothing happened. As expected. If you got any errors here, got back to install Python.

### Variables
Variables allow you to access some data in memory using a name. You are able to seat, read and overwrite these values.

We want to add two numbers. Write the following to assign a value to `a` and `b`:

```python
a = 12
b = 30
```

### Arithmetic Operations
Python supports arithmetic operations. To read the values, calculate an addition and assign it to `answer` write this next:

```python
answer = a + b
```
The right-hand side is evaluated first before the assignments takes place. The right-hand side expressions are evaluated from the left to the right and following order of operations ([PEMDAS][l6]). The result is assigned to the left side.

Run the programm again. Still nothing? Let's change that.

### Data Types
Before you continue, you have to learn about data types.  
Different values are stored differently in memory to improve efficiency and allow specific operations.

The first two important types are:

* [Numeric Types][l5]  
  Python supports integers<sup>[[1]][l1][[2]][l2]</sup>, floating point numbers<sup>[[3]][l3]</sup>, and complex numbers. An integer is assigned to `a` and `b`.
* [Text Sequence Type][l8]  
  Commonly known as [Strings][l9]. This is readable, printable text.

### Built-in Functions
Luckily you don't have to write text output yourself anymore. Python has a lot of built-in functions to serve as simple blocks for your programs. We will use the [print()][l4] function to convert the answer to string and print it in the console. <small>[Google][g1]</small>  
The program should look like this now:

```python
a = 12
b = 30
answer = a + b
print(answer)
```

If you run the program now, it shows you the answer:

```
i:\git\learnprogramming\examples>python calculator.py
42
i:\git\learnprogramming\examples>
```

It is working! That's it. You are now a programmer!  
Yes it is boring and not really useful, but that is easy to fix.

The next step is to replace the hard-coded numbers and to add user input. <small>[Google][g2]</small>  
The [input()][l10] function makes the program wait for user input. It takes a `prompt` string paramter it will show when waiting.  
Call it with a `string` as prompt and assign the result to our variables:

```python
a = input('Number A?')
b = input("Number B?")
answer = a + b
print(answer)
```

Run it and type two number pressing Enter in between. It works, kindof:

```
i:\git\learnprogramming\examples>calculator.py
Number A?12
Number B?30
1230
i:\git\learnprogramming\examples>
```

`input()` returns a string and not a number. Python 'adds' strings by concatenating them. We have to convert them to an `integer` using [int()][l11]. Assign the string return value from `input()` the paramter for `int()`. You can do this directly by writing one function call inside another. You could also use more variables. <small>[Google][g3]</small>

```python
a = int(input('Number A? '))
b = int(input("Number B? "))
answer = a + b
print(answer)
```

**All Done.**

[l1]: https://en.wikipedia.org/wiki/Integer
[l2]: https://en.wikipedia.org/wiki/Integer_(computer_science)
[l3]: https://en.wikipedia.org/wiki/Floating_point
[l4]: https://docs.python.org/3/library/functions.html#print
[l5]: https://docs.python.org/3/library/stdtypes.html#numeric-types-int-float-complex
[l6]: https://en.wikipedia.org/wiki/Order_of_operations
[l7]: https://en.wikipedia.org/wiki/Cd_(command)
[l8]: https://docs.python.org/3/library/stdtypes.html#text-sequence-type-str
[l9]: https://en.wikipedia.org/wiki/String_(computer_science)
[l10]: https://docs.python.org/3/library/functions.html#input
[l11]: https://docs.python.org/3/library/functions.html#int

[g1]: https://encrypted.google.com/search?q=python%20print%20to%20console
[g2]: https://encrypted.google.com/search?q=python+3+get+user+input
[g3]: https://encrypted.google.com/search?q=python%20convert%20string%20to%20integer