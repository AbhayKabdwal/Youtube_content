# Basics of Regular Expressions in Python

Regular expressions (regex or regexp) are powerful tools for pattern matching and text manipulation in Python. They allow you to search for and manipulate strings based on patterns. Here are the basics of working with regular expressions in Python, along with examples for each concept:

## Table of Contents
1. [What are Regular Expressions?](#1-what-are-regular-expressions)
2. [Creating a Regular Expression](#2-creating-a-regular-expression)
3. [Matching Patterns](#3-matching-patterns)
4. [Regular Expression Functions](#4-regular-expression-functions)
5. [Modifiers and Special Characters](#5-modifiers-and-special-characters)
6. [Common Use Cases](#6-common-use-cases)

---

### 1. What are Regular Expressions?

- **Regular Expressions** (regex or regexp) are sequences of characters that define a search pattern.
- They are used to perform operations like search, match, and manipulate strings based on patterns.
- Python's `re` module provides support for working with regular expressions.

### 2. Creating a Regular Expression

- Regular expressions are typically written as strings with specific syntax.
- The most basic regex is a plain string that matches itself.

**Example 1**: A simple regex that matches the word "hello."
```python
import re

pattern = r"hello"
```

**Example 2**: A regex with a more complex pattern that matches email addresses.
```python
pattern = r"\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,7}\b"
```

### 3. Matching Patterns

- Use the `re.search()` function to find the first occurrence of a pattern in a string.

**Example 1**: Matching "world" in the string "Hello, world!"
```python
import re

pattern = r"world"
text = "Hello, world!"
match = re.search(pattern, text)
print(match.group())  # Output: "world"
```

- Use the `re.findall()` function to find all occurrences of a pattern in a string.

**Example 2**: Finding all email addresses in a text.
```python
import re

pattern = r"\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,7}\b"
text = "Emails: alice@example.com, bob@email.net"
matches = re.findall(pattern, text)
print(matches)  # Output: ['alice@example.com', 'bob@email.net']
```

### 4. Regular Expression Functions

- `re.search()`: Searches for a pattern in a string and returns the first match.
- `re.findall()`: Finds all non-overlapping occurrences of a pattern in a string and returns them as a list.
- `re.match()`: Matches a pattern only at the beginning of a string.
- `re.sub()`: Replaces all occurrences of a pattern in a string with a specified replacement.

### 5. Modifiers and Special Characters

- Use special characters and modifiers to create complex patterns.
- Some common special characters include `.` (any character), `*` (zero or more occurrences), `+` (one or more occurrences), and `?` (zero or one occurrence).

**Example 1**: Using `.*` to match any text between "Hello" and "world" (greedy match).
```python
pattern = r"Hello.*world"
text = "Hello, Python world!"
match = re.search(pattern, text)
print(match.group())  # Output: "Hello, Python world"
```

**Example 2**: Using `.*?` for a non-greedy match.
```python
pattern = r"Hello.*?world"
text = "Hello, Python world!"
match = re.search(pattern, text)
print(match.group())  # Output: "Hello, world"
```

### 6. Common Use Cases

- **Validation**: Validate input, like email addresses, phone numbers, or passwords.
- **Extraction**: Extract specific information from a text, like dates, URLs, or numbers.
- **Search and Replace**: Find and replace text based on patterns.
- **Tokenization**: Split text into tokens (words, sentences) based on specific criteria.

## Thank You
- Excited for more ? Subscribe the channel and hit the bell icon to recieve notifications of further contents.

## Next up in the series

- Basics of python continued
    
    + Some useful methods in python

## Contact Me

- Author -- Abhay Kabdwal -- Doctor_Innovator
- **_[Youtube](https://www.youtube.com/@doctor_innovator/featured)_**
- **_[Discord](https://discord.gg/7ydGD3aJ)_**
- **_[Telegram](https://t.me/doctor_innovator)_**