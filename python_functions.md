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
