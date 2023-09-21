# Methods of List, Tuple, Dictionary, and String in Python

Python provides a wide range of built-in methods for manipulating lists, tuples, dictionaries, and strings. Here's an overview of these methods for each data type, along with examples for each method:

## Table of Contents
1. [List Methods](#1-list-methods)
2. [Tuple Methods](#2-tuple-methods)
3. [Dictionary Methods](#3-dictionary-methods)
4. [String Methods](#4-string-methods)

---

### 1. List Methods

#### `append()`
- Adds an element to the end of the list.
```python
my_list = [1, 2, 3]
my_list.append(4)
# Result: [1, 2, 3, 4]
```

#### `extend()`
- Adds elements from an iterable to the end of the list.
```python
my_list = [1, 2, 3]
my_list.extend([4, 5])
# Result: [1, 2, 3, 4, 5]
```

#### `insert()`
- Inserts an element at a specific position.
```python
my_list = [1, 2, 3]
my_list.insert(1, 4)
# Result: [1, 4, 2, 3]
```

#### `remove()`
- Removes the first occurrence of a value from the list.
```python
my_list = [1, 2, 3, 2]
my_list.remove(2)
# Result: [1, 3, 2]
```

#### `pop()`
- Removes and returns an element at a specified index.
```python
my_list = [1, 2, 3]
element = my_list.pop(1)
# Result: element = 2, my_list = [1, 3]
```

#### `index()`
- Returns the index of the first occurrence of a value.
```python
my_list = [1, 2, 3, 2]
index = my_list.index(2)
# Result: index = 1
```

#### `count()`
- Returns the number of occurrences of a value in the list.
```python
my_list = [1, 2, 3, 2]
count = my_list.count(2)
# Result: count = 2
```

#### `sort()`
- Sorts the list in ascending order (in-place).
```python
my_list = [3, 1, 2]
my_list.sort()
# Result: my_list = [1, 2, 3]
```

#### `reverse()`
- Reverses the order of elements in the list (in-place).
```python
my_list = [1, 2, 3]
my_list.reverse()
# Result: my_list = [3, 2, 1]
```

### 2. Tuple Methods

Tuples are immutable, so they have fewer methods compared to lists. Most tuple methods are related to finding values.

#### `count()`
- Returns the number of occurrences of a value in the tuple.
```python
my_tuple = (1, 2, 2, 3)
count = my_tuple.count(2)
# Result: count = 2
```

#### `index()`
- Returns the index of the first occurrence of a value.
```python
my_tuple = (1, 2, 3, 2)
index = my_tuple.index(2)
# Result: index = 1
```

***Although tuples are immutable they can me accessed and altered using tuple unpacking***

- ###  What is Tuple Unpacking?

    - **Tuple Unpacking** is the process of extracting values from a tuple and assigning them to separate variables in a single operation.
    
    - It is a convenient way to work with the elements of a tuple without needing to access them by index.

- ###  Basic Tuple Unpacking

    - To perform basic tuple unpacking, you simply assign the values of the tuple to the variables on the left side of the assignment operator (`=`).

**Example** : Basic tuple unpacking with two variables.
```python
my_tuple = (1, 2)
x, y = my_tuple
# Now, x = 1 and y = 2
```

**Example** : Basic tuple unpacking with three variables.
```python
my_tuple = ('Alice', 30, 'New York')
name, age, city = my_tuple
# Now, name = 'Alice', age = 30, and city = 'New York'
```

- ### Extended Tuple Unpacking

    - You can use an asterisk (`*`) to assign the remaining values of a tuple to a single variable.

**Example** : Extended tuple unpacking with an asterisk.
```python
my_tuple = (1, 2, 3, 4, 5)
first, *rest, last = my_tuple
# Now, first = 1, rest = [2, 3, 4], and last = 5
```

- ### Using Tuple Unpacking in Functions

    - Tuple unpacking is often used in functions to return multiple values.

**Example**: Using tuple unpacking in a function.
```python
def get_coordinates():
    return (3, 4)

x, y = get_coordinates()
# Now, x = 3 and y = 4
```

- ### Swapping Variables

    - Tuple unpacking provides a concise way to swap the values of two variables without needing a temporary variable.

**Example**: Swapping variables using tuple unpacking.
```python
x = 5
y = 10
x, y = y, x
# Now, x = 10 and y = 5
```

- ### Ignoring Unwanted Values

    - If you don't need all the values in a tuple, you can use `_` (underscore) to ignore unwanted values.

**Example**: Ignoring unwanted values using tuple unpacking.
```python
my_tuple = (1, 2, 3, 4, 5)
x, _, _, _, y = my_tuple
# Now, x = 1 and y = 5 (values 2, 3, and 4 are ignored)
```

Tuple unpacking is a versatile feature in Python that simplifies code readability and can make your code more expressive when working with tuples.

### 3. Dictionary Methods

#### `keys()`
- Returns a list of all keys in the dictionary.
```python
my_dict = {'name': 'Alice', 'age': 30}
keys = my_dict.keys()
# Result: keys = ['name', 'age']
```

#### `values()`
- Returns a list of all values in the dictionary.
```python
my_dict = {'name': 'Alice', 'age': 30}
values = my_dict.values()
# Result: values = ['Alice', 30]
```

#### `items()`
- Returns a list of key-value pairs (tuples) in the dictionary.
```python
my_dict = {'name': 'Alice', 'age': 30}
items = my_dict.items()
# Result: items = [('name', 'Alice'), ('age', 30)]
```

#### `get()`
- Returns the value for a specified key, or a default value if the key does not exist.
```python
my_dict = {'name': 'Alice', 'age': 30}
age = my_dict.get('age', 0)
# Result: age = 30
```

#### `pop()`
- Removes and returns the value for a specified key.
```python
my_dict = {'name': 'Alice', 'age': 30}
name = my_dict.pop('name')
# Result: name = 'Alice', my_dict = {'age': 30}
```

#### `update()`
- Updates the dictionary with key-value pairs from another dictionary.
```python
my_dict = {'name': 'Alice', 'age': 30}
my_dict.update({'city': 'New York', 'age': 31})
# Result: my_dict = {'name': 'Alice', 'age': 31, 'city': 'New York'}
```

### 4. String Methods

#### `lower()`
- Converts all characters in a string to lowercase.
```python
my_string = "Hello, World!"
lower_case = my_string.lower()
# Result: lower_case = "hello, world!"
```

#### `upper()`
- Converts all characters in a string to uppercase.
```python
my_string = "Hello, World!"
upper_case = my_string.upper()
# Result: upper_case = "HELLO, WORLD!"
```

#### `strip()`
- Removes leading and trailing whitespace characters from a string.
```python
my_string = "   Hello, World!   "
stripped = my_string.strip()
# Result: stripped = "Hello, World!"
```

#### `split()`
- Splits a string into a list of substrings based on a specified delimiter.
```python
my_string = "apple,banana,cherry"
my_list = my_string.split(",")
# Result: my_list = ['apple', 'banana', 'cherry']
```

#### `join()`
- Joins elements of an iterable (e.g., a list) into a single string using the string as a delimiter.
```python
my_list = ['apple', 'banana', 'cherry']
my_string = ",".join(my_list)
# Result: my_string = "apple,banana,cherry"
```

#### `replace()`
- Replaces all occurrences of a substring with another substring.
```python
my_string = "Hello, World!"
new_string = my_string.replace("World", "Python")
# Result: new_string = "Hello, Python!"
```

## Thank You
- Excited for more ? Subscribe the channel and hit the bell icon to recieve notifications of further contents.

## Next up in the series

- Automation Projects

## Contact Me

- Author -- Abhay Kabdwal -- Doctor_Innovator
- **_[Youtube](https://www.youtube.com/@doctor_innovator/featured)_**
- **_[Discord](https://discord.gg/7ydGD3aJ)_**
- **_[Telegram](https://t.me/doctor_innovator)_**