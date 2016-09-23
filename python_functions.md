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

### Local variable
In many other programming languages, variables are treated as global if not otherwise declared. But python deals variables other way around - They are local, if not otherwise declared.

Why python has this approach: In general, declaring global variable is a bad practice and should be avoided. Instead of declaring global variable, it is better to utilize a parameter for getting a value into a function or return value to get it out.

Let's write a program where you can define a local variable in "ex8.py":
```
# declare a variable
x = 50

def func(x):
    print('x is', x)
    x = 2
    print('Changed local x to', x)

func(x)
print('x is still', x)
```
If you run this program, you should get an output like this:
```
$ python ex9.py
('x is', 50)
('Changed local x to', 2)
('x is still', 50)
```
### Explation for local variable program
The first time that we print the value of the name x with the first line in the function's body, Python uses the value of the parameter declared in the main block, above the function definition.

Next, we assign the value 2 to x. The name x is local to our function. So, when we change the value of x in the function, the x defined in the main block remains unaffected.

With the last print statement, we display the value of x as defined in the main block, thereby confirming that it is actually unaffected by the local assignment within the previously called function.

### Global variable
As I mentioned earlier, any variable assigned in a function is local to that function, unless it is specifically declared global. Let's write the same program which we wrote in local variable section but will define it a global function "ex10.py":
```
# Assign a value to a variable
x = 50

# Define it global
def func():
    global x

    print('x is', x)
    x = 2
    print('Changed global x to', x)

func()
print('Value of x is', x)
```
If you run this program, your output some look like this:
```
$ python ex10.py
('x is', 50)
('Changed global x to', 2)
('Value of x is', 2)
```

### Practice drills and recommendation
Do this experiment before moving to next chapter.
- Write same program with different variables.
- Make mistake knowingly and analyse the errors.
- Do Googling with a keywords like - functions, local variables in python, global variables in python.
- Write comment for every single line of code. 
