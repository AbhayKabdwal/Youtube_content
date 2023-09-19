# Conditional Statements in Python

Conditional statements are essential components of programming languages like Python. They allow you to control the flow of your code based on specific conditions. In Python, you can use the following conditional statements:

## 1. **if Statement**

The `if` statement is used to execute a block of code only if a specified condition is true. If the condition is false, the code block is skipped.

**Syntax:**

```python
if condition:
    # Code to execute if the condition is true
```

**Example 1:**

```python
x = 10
if x > 5:
    print("x is greater than 5")
```

**Example 2:**

```python
age = 15
if age >= 18:
    print("You are an adult")
else:
    print("You are a minor")
```

## 2. **elif Statement**

The `elif` statement allows you to check multiple conditions sequentially. It is used when you want to test multiple conditions and execute different code blocks based on the first true condition.

**Syntax:**

```python
if condition1:
    # Code to execute if condition1 is true
elif condition2:
    # Code to execute if condition2 is true
else:
    # Code to execute if none of the conditions are true
```

**Example 1:**

```python
score = 75
if score >= 90:
    print("A")
elif score >= 80:
    print("B")
elif score >= 70:
    print("C")
else:
    print("F")
```

**Example 2:**

```python
num = -5
if num > 0:
    print("Positive")
elif num < 0:
    print("Negative")
else:
    print("Zero")
```

## 3. **else Statement**

The `else` statement is used to define a block of code that will be executed if the condition in the `if` statement is false.

**Syntax:**

```python
if condition:
    # Code to execute if the condition is true
else:
    # Code to execute if the condition is false
```

**Example 1:**

```python
x = 3
if x % 2 == 0:
    print("Even")
else:
    print("Odd")
```

**Example 2:**

```python
password = "secret"
if password == "password123":
    print("Access granted")
else:
    print("Access denied")
```

These are the fundamental conditional statements in Python. They allow you to make decisions and control the flow of your program based on specific conditions. Depending on the situation, you can use `if`, `elif`, and `else` statements to create complex decision-making logic in your Python programs.


## Thank You
- Excited for more ? Subscribe the channel and hit the bell icon to recieve notifications of further contents.

## Next up in the series

- Basics of python continued
    
    + Loop statements


## Contact Me

- Author -- Abhay Kabdwal -- Doctor_Innovator
- **_[Youtube](https://www.youtube.com/@doctor_innovator/featured)_**
- **_[Discord](https://discord.gg/7ydGD3aJ)_**
- **_[Telegram](https://t.me/doctor_innovator)_**