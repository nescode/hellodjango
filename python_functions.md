## What you will learn in this section
You’ll learn about how to define a function and resuse that in your program.

### Introduction
Functions are reusable pieces of programs. They allow you to give a name to a block of statements, allowing you to run that block using the specified name anywhere in your program and any number of times. This is known as calling the function. There are several built-in functions in python which you use regularly while writing a program.
Why you should write and user functions in program - It allows us to order your code, make it more readable, reuse it and save some time. A simple function can be in this format:
```
def hello_django():
    print "Hello Django!"
```
Let's write a program "ex7.py" by defining a function and calling it in program:
```
# Defining a function
def hello_django():
    print('Hello Django!')
# End of function

hello_django()  # call the function
```
Let's run this program, your output should come like this
```
$ python ex7.py
Hello Django!
```
### Functions parameters
You can give value to your functions to do something. Every functions in python receives a predefined number of arguments, if declared normally. A very basic function with parameters looks like this:
```
def hello_django(first, second, third):
    # do something with the 3 variables
    ...
```
Parameters like "first", "second" and "third" are just like variables except that the values of these variables are defined when we call the function and are already assigned values when the function runs.

Parameters are specified within the pair of parentheses in the function definition, separated by commas. Let's write a simple function with parameter program in "ex8.py":
```
# defining a function
def print_max(a, b):
    if a > b:
        print(a, 'is maximum')
    elif a == b:
        print(a, 'is equal to', b)
    else:
        print(b, 'is maximum')

# directly pass literal values
print_max(3, 4)

x = 5
y = 7

# pass variables as arguments
print_max(x, y)
```
Let's run this program, your output should be like this:
```
$ python ex8.py
(4, 'is maximum')
(7, 'is maximum')
```
