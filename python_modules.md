## What you will learn in this section
You’ll learn about how to define various function and resuse them in your program.

### Introduction
In our previous chapter, we seen how to write a block of code(function) and call in a program. How about defining a various function and calling them in a program. Yes, you can do this. Therefore, you can define module in a simple one line - module is a file containing Python definitions and statements.

There are various methods of writing modules, but the simplest way is to
- Create a file with a .py extension that contains functions and variables.
- Write the modules in the native language in which the Python interpreter itself was written.

Post writing a module, you can import it in another program to make use of its functionality. This is how we can use the Python standard library as well.

### Start with basic modules
Let's write a most basic modules and import it. Create a file "ex11.py" and write below program:
```
import sys

print('The command line arguments are:')
for i in sys.argv:
    print(i)

print('\n\nThe PYTHONPATH is', sys.path, '\n')
```
Then open your terminal and import "ex11.py" (without quote)
```
$ python ex11.py
The command line arguments are:
ex11.py
('\n\nThe PYTHONPATH is', ['/home/nescode/project/bitbucketsunil/hdpython', '/usr/lib/python2.7', '/usr/lib/python2.7/plat-x86_64-linux-gnu', '/usr/lib/python2.7/lib-tk', '/usr/lib/python2.7/lib-old', '/usr/lib/python2.7/lib-dynload', '/usr/local/lib/python2.7/dist-packages', '/usr/lib/python2.7/dist-packages', '/usr/lib/python2.7/dist-packages/gtk-2.0'], '\n')
```
Let's explain what we did above:
We import the sys module using import statement. Now you would be surprised what is sys module? The sys module contains functionality related to the python interpreter and its environment i.e. the system. When python executes the import sys statement, it looks for the sys module.and print the path.

### `from.. import` statement
Let's say, you want to directly `import` the argv variable into your program, then you can use the `from sys` import argv statement. Let's create a new file named "ex12.py" and type this program.

```
from math import sqrt
print("Square root of 16 is", sqrt(16))
```
Run you program and see the results it display
```
$ python ex12.py
('Square root of 16 is', 4.0)
```

### A module's `__name__`
Every module has a name and statements in a module. This is handy for the particular purpose of figuring out whether the module is being run standalone or being imported. As mentioned previously, when a module is imported for the first time, the code it contains gets executed. We can use this to make the module behave in different ways depending on whether it is being used by itself or being imported from another module. This can be achieved using the `__name__` attribute of the module.

Let's create another file named "ex13.py" and write this code

```
if __name__ == '__main__':
    print('This program is being run by itself')
else:
    print('I am being imported from another module')
```
Now, run this code in terminal
```
$ python ex13.py
This program is being run by itself
```
Every Python module has its `__name__` defined. If this is `__main__`, that implies that the module is being run standalone by the user and we can take appropriate actions.

### Practice drills and recommendation
Do this experiment before moving to next chapter.

- Read modules chapter from official python documentation https://docs.python.org/2/tutorial/modules.html
- Make mistake knowingly and analyse the errors.
- Do Googling with a keywords like - Python modules, Import a module, Import local path through python module.
- Write comment for every single line of code.
