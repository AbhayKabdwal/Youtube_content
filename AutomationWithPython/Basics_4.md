# Loop Statements in Python

Loop statements in Python allow you to repeat a block of code multiple times, making it easier to perform repetitive tasks. There are two primary types of loop statements in Python: `for` and `while` loops.

## 1. **`for` Loop**

A `for` loop is used to iterate over a sequence (e.g., a list, tuple, string, or range) or any iterable object. It executes a block of code for each item in the sequence.

**Syntax:**

```python
for item in iterable:
    # Code to execute for each item
```

**Example 1: Looping Through a List**

```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
```

**Example 2: Using `range()` to Generate a Sequence**

```python
for i in range(1, 5):
    print(i)
```

## 2. **`while` Loop**

A `while` loop is used to repeatedly execute a block of code as long as a specified condition is true. It checks the condition before each iteration.

**Syntax:**

```python
while condition:
    # Code to execute as long as the condition is true
```

**Example 1: Counting Down from 5**

```python
count = 5
while count > 0:
    print(count)
    count -= 1
```

**Example 2: User Input Validation**

```python
user_input = ""
while user_input != "quit":
    user_input = input("Enter a command ('quit' to exit): ")
    print(f"You entered: {user_input}")
```

These loop statements are fundamental in Python and are used extensively to perform tasks that involve repetitive actions. Whether you need to process items in a collection or repeatedly execute code based on a condition, `for` and `while` loops provide the necessary tools to handle various iteration scenarios.

## Thank You
- Excited for more ? Subscribe the channel and hit the bell icon to recieve notifications of further contents.

## Next up in the series

- Basics of python continued
    
    + Functions


## Contact Me

- Author -- Abhay Kabdwal -- Doctor_Innovator
- **_[Youtube](https://www.youtube.com/@doctor_innovator/featured)_**
- **_[Discord](https://discord.gg/7ydGD3aJ)_**
- **_[Telegram](https://t.me/doctor_innovator)_**