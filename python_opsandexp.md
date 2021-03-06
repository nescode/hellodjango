## What you will learn in this section
You’ll learn about expressions, operators, sequences, and more.

### Introduction
Most statements (logical lines) that you write in any programming language contain expressions. A simple example of an expression is 2 + 3. An expression can be broken down into operators and operands.

**Operators and operands:** Operators are functionality that do something and can be represented by symbols such as + or by special keywords. Operators require some data to operate on and such data is called operands. In this case, 2 and 3 are the operands. Some of the well known operators with descriptions and examples are:

SL | OPERATORS | DESCRIPTIONS | EXAMPLE
--------------- | ------------ | ------------- | ----------------
1 | + (plus) | Add two number | 3 + 5 gives 8. 'a' + 'b' gives 'ab'
2 | - (minus) | Gives the subtraction of one number from the other | 50 - 24 gives 26
3 | * (multiply) | Gives the multiplication of the two numbers or returns the string repeated that many times. | 2 * 3 gives 6. 'la' * 3 gives 'lalala'
4 | ** (power) | Returns x to the power of y | 3 ** 4 gives 81
5 | / (divide) | Divide x by y | 13 / 3 gives 4.333333333333333
6 | // (divide and floor) | Divide x by y and round the answer down to the nearest whole number | 13 // 3 gives 4
7 | % (modulo) | Returns the remainder of the division | 13 % 3 gives 1
8 | << (left shift) | Shifts the bits of the number to the left by the number of bits specified. | 2 << 2 gives 8
9 | >> (right shift) | Shifts the bits of the number to the right by the number of bits specified. | 11 >> 1 gives 5
10 | & (bit-wise AND) | Bit-wise AND of the numbers | 5 & 3 gives 1.
11 | ^ (bit-wise XOR) | Bitwise XOR of the numbers | 5 ^ 3 gives 6
12 | ~ (bit-wise invert) | The bit-wise inversion of x is -(x+1) | ~5 gives -6
13 | < (less than) | Returns whether x is less than y. | 5 < 3 gives False
14 | > (greater than) | Returns whether x is greater than y | 5 > 3 returns True
15 | <= (less than or equal to) | Returns whether x is less than or equal to y | x = 3; y = 6; x <= y returns True
16 | >= (greater than or equal to) | Returns whether x is greater than or equal to y | x = 4; y = 3; x >= 3 returns True
17 | == (equal to) | Compares if the objects are equal | x = 2; y = 2; x == y returns True
18 | != (not equal to) | Compares if the objects are not equal | x = 2; y = 3; x != y returns True
19 | not (boolean NOT) | If x is True, it returns False. If x is False, it returns True. | x = True; not x returns False.
20 | and (boolean AND) | x and y returns False if x is False, else it returns evaluation of y | x = False; y = True; x and y returns False since x is False.
21 | or (boolean OR) | If x is True, it returns True, else it returns evaluation of y | x = True; y = False; x or y returns True

### Evaluation order
In case of expression such as 2 + 3 * 4, multiplication operator has higher precedence than the addition operator.
The following table gives the precedence table for Python, from the lowest precedence (least binding) to the highest precedence (most binding). This means that in a given expression, Python will first evaluate the operators and expressions lower in the table before the ones listed higher in the table. Operators in the same box group left to right (except for exponentiation, which groups from right to left). Table reference [Python evaluation order](https://docs.python.org/3/reference/expressions.html#operator-precedence)

SL | OPERATOR | DESCRIPTIONS
-------- | --------- | -----------
1 | lambda | Lambda expression
2 | if – else | Conditional expression
3 | or | Boolean OR
4 | and | Boolean AND
5 | not x | Boolean NOT
6 | in, not in, is, is not, <, <=, >, >=, !=, == | Comparisons, including membership tests and identity tests
7 | ^ | Bitwise XOR
8 | & | Bitwise AND
9 | <<, >> | Shifts
10 | +, - | Addition and subtraction
11 | +x, -x, ~x | Positive, negative, bitwise NOT
12 | ** | Exponentiation
13 | await x | Await expression
14 | x[index], x[index:index], x(arguments...), x.attribute | Subscription, slicing, call, attribute reference
15 | (expressions...), [expressions...], {key: value...}, {expressions...} | Binding or tuple display, list display, dictionary display, set display

### Associativity
Operators are usually associated from left to right. This means that operators with the same precedence are evaluated in a left to right manner. For example, 2 + 3 + 4 is evaluated as (2 + 3) + 4.
Open you atom editor and create a file "ex2.py" and measure area and Perimeter of a rectangle like this:
```
# Assigning value in a variales named length and breadth
length = 5
breadth = 2

# Calculating, printing area and Perimeter
area = length * breadth
print('Area is', area)
print('Perimeter is', 2 * (length + breadth))
```
Now, open your terminal and run, your output should be similar to this:
```
$ python ex2.py
Area is 10
Perimeter is 14
```

### Study drills and recommendation
We have seen how operators, operands and expressions - these are the basic building blocks of any program. If you are willing to be a good programmer then you must have sound knowledge of operations and expressions. Keep practice by doing various operations.
- Read again and again, if you have missed something.
- Find something you need to calculate and create another .py file and write your program.
- Do googling, if you stuck somewhere.
- Use an old method of writing a program on paper, this will help you avoid small mistakes since all modern IDE give code hints which shrinking developer common sense.
