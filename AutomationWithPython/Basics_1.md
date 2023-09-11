# Python Basics

## Variables

- Variables are used to store data in Python.
- You can create a variable and assign a value to it using the assignment operator `=`.

<br>

```py
# Example: Creating and assigning values to variables

name = "John"
age = 30
```


- Variable names should follow certain rules:
    - Must start with a letter (a-z, A-Z) or underscore (_).
    - Can contain letters, numbers, and underscores.
    - Variables are case-sensitive.


```py
# Example: Variable naming

first_name = "Alice"
_last_name = "Smith"
```

## Data Types

Python has various data types to represent different types of values.
Common data types include integers, floating-point numbers, strings, and lists.

<br>

```py
# Example: Data types

age = 25         # Integer
height = 5.8     # Float
name = "Alice"  # String
fruits = ["apple", "banana", "cherry"]  # List
```
<br>

# Operators in Python
Operators are special symbols that perform some operations on values or variables. Python supports various types of operators such as:

Arithmetic operators: these operators are used to perform mathematical calculations such as addition, subtraction, multiplication, division, etc. For example:

```py
# Example : Numerical operators in python

x = 10
y = 5

print(x + y) # 15
print(x - y) # 5
print(x * y) # 50
print(x / y) # 2.0
print(x % y) # 0 (remainder of x / y)
print(x ** y) # 100000 (x raised to the power of y)
print(x // y) # 2 (integer division of x / y)
```
<br>

## Comparison operators: 

These operators are used to compare two values or variables and return a boolean value (True or False). For example:

```py
# Example : Comparison operators in python

x = 10
y = 5

print(x == y) # False (x is equal to y)
print(x != y) # True (x is not equal to y)
print(x > y) # True (x is greater than y)
print(x < y) # False (x is less than y)
print(x >= y) # True (x is greater than or equal to y)
print(x <= y) # False (x is less than or equal to y)
```
<br>

## Logical operators: 
These operators are used to combine two or more boolean expressions and return a boolean value. The logical operators in Python are and, or, and not. For example:

```py
# Example : Logical operators in python

x = True
y = False

print(x and y) # False (x and y are both True)
print(x or y) # True (x or y is True)
print(not x) # False (the opposite of x)
```
<br>

## Assignment operators: 

These operators are used to assign a value to a variable. The basic assignment operator is =. There are also some shorthand assignment operators that combine an arithmetic or bitwise operator with an assignment. For example:

```py
# Example : Assignment operators in python

x = 10 # assign 10 to x
x += 5 # equivalent to x = x + 5
x -= 5 # equivalent to x = x - 5
x *= 5 # equivalent to x = x * 5
x /= 5 # equivalent to x = x / 5
x %= 5 # equivalent to x = x % 5
x **= 5 # equivalent to x = x ** 5
x //= 5 # equivalent to x = x // 5
```
<br>

## Bitwise operators: 

These operators are used to perform operations on binary numbers (represented as bits). The bitwise operators in Python are & (bitwise and), | (bitwise or), ^ (bitwise xor), ~ (bitwise not), << (left shift), and >> (right shift). For example:

```py
# Example : Bitwise operators in python

x = 10 # binary representation: 1010
y = 5 # binary representation: 0101

print(x & y) # 0 (bitwise and: 1010 & 0101 = 0000)
print(x | y) # 15 (bitwise or: 1010 | 0101 = 1111)
print(x ^ y) # 15 (bitwise xor: 1010 ^ 0101 = 1111)
print(~x) # -11 (bitwise not: ~1010 = -1011)
print(x << 2) # 40 (left shift: 1010 << 2 = 101000)
print(x >> 2) # 2 (right shift: 1010 >> 2 = 0010)
```

<br>

# Input and Output in Python

Input and output refers to the process of getting data from the user or displaying data to the user. Python provides some built-in functions for input and output such as:

- input(): this function takes a string as an argument and returns the user’s input as a string. For example:

```py
# Example : Taking input in python

name = input("What is your name? ") # get the user's name
age = input("How old are you? ") # get the user's age
print("Hello, " + name + ". You are " + age + " years old.") # print a greeting message
```

The output of the above code depends on what the user enters. For example:

```sh
What is your name? Alice
How old are you? 20
Hello, Alice. You are 20 years old.
```

<br>

- print(): this function takes one or more arguments and prints them to the standard output (usually the screen). The arguments can be separated by commas or concatenated by +. For example:

```py
# Example : Printing the output on screen in python

x = 10
y = 20
z = x + y

print(x, "+", y, "=", z) # print with commas
print(str(x) + " + " + str(y) + " = " + str(z)) # print with concatenation
```

The output of the above code is:

```sh
10 + 20 = 30
10 + 20 = 30
```

<br>

-  We can also use some formatting options to customize the output of the print() function. For example, we can use the sep parameter to specify the separator between the arguments, and the end parameter to specify the end character of the output. For example:

```py
# Example : Parameters of print function in python

print(x, y, z, sep=" - ") # use "-" as separator
print(x, y, z, end=".\n") # use "." and newline as end character
```

The output of the above code is:

```sh
10 - 20 - 30
10 20 30.
```

<br>

- We can also use the format() method or the f-string syntax to insert values into placeholders in a string. For example:

```py
# Example : Formatted string method of output in python

print("The value of x is {}".format(x)) # use format() method
print(f"The value of y is {y}") # use f-string syntax
```

The output of the above code is:

```sh
The value of x is 10
The value of y is 20
```

## Thank You
- Excited for more ? Subscribe the channel and hit the bell icon to recieve notifications of further contents.

## Next up in the series

- Basics of python continued
    
    + Conditional statements

## Contact Me

- Author -- Abhay Kabdwal -- Nerdy_Innovator
- **_[Youtube](https://www.youtube.com/@abhaykabdwal2911/featured)_**
- **_[Discord](https://discord.gg/7ydGD3aJ)_**
- **_[Telegram](https://t.me/doctor_innovator)_**