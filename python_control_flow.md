## What you will learn in this section
You’ll learn about how to change flow of execution in python, take some decisions and do different things depending on different situations.

### Introduction
A simple program like in python basic chapter, getting executed from top-down order. How about if we can change the order of execution of program by using some conditions depending upon situations. For an example, let's say if your score card is 100 then print "Awesome" else "Let's study again". You can achieve this by using control flow statements.

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
Let's write another program in "ex4.py" and run:
```
number = 23
guess = int(input('Enter an integer : '))

if guess == number:
    # New block starts here
    print('Congratulations, you guessed it.')

elif guess < number:
    # Another block
    print('No, it is a little higher than that')
    # You can do whatever you want in a block.

else:
    print('No, it is a little lower than that')
    # you must have guessed > number to reach here

print('Done')
# This last statement is always executed,
# after the if statement is executed.
```
Let's run the program, you should see output like this
```
$ python ex4.py
Enter an integer : 25
No, it is a little lower than that
Done
```
### While statement
The while statement allows you to repeatedly execute a block of statements as long as a condition is true. You can also consider it as an example of a looping statement. A while statement can have an optional else clause.
Let's write another program in "ex5.py" for while loop and run:
```
number = 23
running = True

while running:
    guess = int(input('Enter an integer : '))

    if guess == number:
        print('Congratulations, you guessed it.')
        # this causes the while loop to stop
        running = False
    elif guess < number:
        print('No, it is a little higher than that.')
    else:
        print('No, it is a little lower than that.')
else:
    print('The while loop is over.')
    # Do anything else you want to do here

print('Done')
```
Let's run the program, you should see output like this
```
$ python ex5.py
Enter an integer : 30
No, it is a little lower than that.
Enter an integer : 25
No, it is a little lower than that.
Enter an integer : 18
No, it is a little higher than that.
Enter an integer : 23
Congratulations, you guessed it.
The while loop is over.
Done
```
### The for loop
The for..in statement is another looping statement which iterates over a sequence of objects i.e. go through each item in a sequence. Let's write another program in "ex6.py" and run it.
```
# For loop
for i in range(1, 5):
    print(i)
else:
    print('The for loop is over')
```
Let's run this program, you should see output like this:
```
$ python ex6.py
1
2
3
4
The for loop is over
```

### Practice drills and recommendation
Do this experiment before moving to next chapter.
- Why does the code under the if need to be indented four spaces?
- What happens if it isn’t indented?
- Try some more complex boolean expression.
- What happens if you change the initial variables for boys, girls and rose?
- Knwoingly do a spelling mistake in "elif" and run the program and analyse error in terminal.
- Remove indentation in ex5.py and run the program. If you get an error, google it.
- In above program, write a description for every line.

Well, if it's too much for you then take a break. Have some fun and come back.
