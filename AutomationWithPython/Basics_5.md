# Functions in Python

Functions in Python are reusable blocks of code that perform specific tasks. They are essential for organizing and modularizing code. Functions can take input, process it, and return output. There are two main types of functions in Python: built-in functions and user-defined functions.

## 1. **Built-in Functions**

Python provides a wide range of built-in functions that are readily available for common tasks. Here are three examples:

### a. `print()`

The `print()` function is used to display text or variables on the console.

**Example 1: Displaying Text**

```python
print("Hello, world!")
```

**Example 2: Displaying Variables**

```python
x = 10
y = 20
print("Sum:", x + y)
```

### b. `len()`

The `len()` function is used to determine the length of a sequence, such as a string, list, or tuple.

**Example 1: Finding the Length of a String**

```python
text = "Python is fun!"
length = len(text)
print("Length:", length)
```

**Example 2: Finding the Length of a List**

```python
numbers = [1, 2, 3, 4, 5]
count = len(numbers)
print("Count:", count)
```

### c. `max()`

The `max()` function is used to find the maximum value from a sequence or a set of arguments.

**Example 1: Finding the Maximum Value in a List**

```python
scores = [85, 92, 78, 95, 88]
highest_score = max(scores)
print("Highest Score:", highest_score)
```

**Example 2: Finding the Maximum of Multiple Values**

```python
x = 45
y = 72
z = 60
max_value = max(x, y, z)
print("Maximum Value:", max_value)
```

## 2. **User-Defined Functions**

User-defined functions are created by the programmer to perform specific tasks as needed. They enhance code modularity and reusability. Here are three examples:

### a. `add_numbers()`

A simple user-defined function to add two numbers.

**Example 1: Adding Two Numbers**

```python
def add_numbers(a, b):
    return a + b

result = add_numbers(5, 3)
print("Sum:", result)
```

**Example 2: Adding Two Floating-Point Numbers**

```python
def add_floats(x, y):
    return x + y

result = add_floats(3.5, 2.1)
print("Sum:", result)
```

### b. `is_even()`

A user-defined function to check if a number is even.

**Example 1: Checking if a Number is Even**

```python
def is_even(number):
    return number % 2 == 0

result = is_even(6)
print("Is Even:", result)
```

**Example 2: Checking Oddness**

```python
def is_odd(number):
    return not is_even(number)

result = is_odd(9)
print("Is Odd:", result)
```

### c. `calculate_average()`

A user-defined function to calculate the average of a list of numbers.

**Example 1: Calculating the Average of a List**

```python
def calculate_average(numbers):
    total = sum(numbers)
    count = len(numbers)
    return total / count

scores = [85, 92, 78, 95, 88]
average = calculate_average(scores)
print("Average Score:", average)
```

**Example 2: Calculating the Average of Grades**

```python
def grade_average(grades):
    grade_points = {"A": 4.0, "B": 3.0, "C": 2.0, "D": 1.0, "F": 0.0}
    total_points = sum(grade_points[grade] for grade in grades)
    count = len(grades)
    return total_points / count

student_grades = ["A", "B", "C", "A", "B"]
average = grade_average(student_grades)
print("Average GPA:", average)
```

Functions are a fundamental concept in Python programming, allowing you to encapsulate and reuse code efficiently. Built-in functions provide a wide range of functionality, while user-defined functions empower you to create custom logic tailored to your specific needs.

## Thank You
- Excited for more ? Subscribe the channel and hit the bell icon to recieve notifications of further contents.

## Next up in the series

- Basics of python continued
    
    + Modules and libraries


## Contact Me

- Author -- Abhay Kabdwal -- Doctor_Innovator
- **_[Youtube](https://www.youtube.com/@doctor_innovator/featured)_**
- **_[Discord](https://discord.gg/7ydGD3aJ)_**
- **_[Telegram](https://t.me/doctor_innovator)_**