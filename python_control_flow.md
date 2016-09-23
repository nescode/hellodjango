## What you will learn in this section
You’ll learn about how to change flow of execution in python, take some decisions and do different things depending on different situations.

### Introduction
A simple program like in python basic chapter, getting executed from top-down order. How about if we can change the order of execution of program by using some conditions depending upon situations. For an example, let's say if your score card is 100 then print "Awesome" else "Let's study again.". You can achieve this by using control flow statements.

There are three control flow statements in Python - if, for and while. Lets create a new file "ex3.py" and type this basic program:
```
# Assign a variable
boys = 20
girls = 30
rose = 15

# Compare the value
if boys < girls:
  print "Too many girls are there compare to boys."

if boys > girls:
  print "Not many girls are there compare to boys."

rose += 5

if boys >= rose:
  print "Boys are greater than or equal to rose."

if boys <= rose:
  print "Boys are less than or equal to rose."

if boys == rose:
  print "Boys are equal to rose."
```
You should see output like below:
```
$ python ex3.py
Too many girls are there compare to boys.
Boys are greater than or equal to rose.
Boys are less than or equal to rose.
Boys are equal to rose.
```
