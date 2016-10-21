## What you will learn in this section
You’ll learn about how to store data in your program.

### Introduction
 Data strucutre is an structures which can hold some data together. In other words they are used to store a collection of related data. There are four built-in data structures in Python:
 - list
 - tuple
 - dictionary
 - set

We will see how to use each of them and how they help us store data properly.

### List
In python, A `list` is a data structure that holds an ordered collection of items i.e. you can store a sequence of items in a list.

This is easy to imagine if you can think of a shopping list where you have a list of items to buy, except that you probably have each item on a separate line in your shopping list whereas in Python you put commas in between them.

The list of items should be enclosed in square brackets so that Python understands that you are specifying a list. Once you have created a list, you can add, remove or search for items in the list. Since we can add and remove items, we say that a list is a mutable data type i.e. this type can be altered.

List can have any number of items and they may be of different types (integer, float, string etc.).

#### Nested list
A list can even have another list as an item. That list are called nested list.

Let's do some practice to understand `list` in much easier way. In your python shell, define a variable called "django" and store some elements value into it.
```
# empty list
django = []

# list of integers
django = [1, 2, 3]

# list with mixed datatypes
django = [1, "Hello", 3.4]

# nested list
django = ["mouse", [8, 4, 6]]
```

### Accessing Values in Lists
To access values in lists, use the square brackets for slicing along with the index or indices to obtain value available at that index. For example:
```
>>> django = [1, 2, 3]
>>> print django[0]
1
>>> django = ["mouse", [8, 4, 6]]
>>> print django[0]
mouse
>>>
```

### Updating Lists
You can update single or multiple elements of lists by giving the slice on the left-hand side of the assignment operator, and you can add to elements in a list with the append() method. Let's open a terminal and update a list.
```
>>> nescode = ["hello django", "apps", "ERP"]
>>> print nescode[2]
ERP
>>> nescode[2] = "apps"
>>> print nescode[2]
apps
>>>
```
In above example, you have seen how to update list in python. Similarly, you can delete and index. There are various built-in list function and method in python, some of the examples are:

SL | FUNCTION | DESCRIPTION
--- | ------- | -----------
1 | cmp(list1, list2) | Compares elements of both lists.
2 | len(list) | Gives the total length of the list.
3 | max(list) | Returns item from the list with max value.
4 | min(list) | Returns item from the list with min value.
5 | list(seq) | Converts a tuple into list.
