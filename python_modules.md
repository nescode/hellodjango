## What you will learn in this section
You’ll learn about how to define various function and resuse them in your program.

### Introduction
In our previous chapter, we seen how to write a block of code(function) and call in program. How about defining a various function and calling them in a program. Yes, you can do this. Therefore, you can define module in a simple one line - module is a file containing Python definitions and statements.

There are various methods of writing modules, but the simplest way is to
- Create a file with a .py extension that contains functions and variables.
- Write the modules in the native language in which the Python interpreter itself was written.

Post writing a module, you can import it in another program to make use of its functionality. This is how we can use the Python standard library as well.

### Start with basic modules
Let's write a most basic modules and import it. Create a file "ex11.py" and write below program:
```
def hello_django():
   print "Hello Django, you are awesome."
```
Then open your terminal and import "ex11.py" (without quote)
