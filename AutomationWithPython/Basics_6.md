# Modules and Libraries in Python

Modules and libraries in Python are essential components that extend the functionality of the language by providing pre-defined code, functions, and classes for various purposes. They promote code reuse, organization, and modularity.

## 1. **Modules**

A module is a Python script containing functions, classes, and variables that can be imported and used in other Python scripts. Modules help organize code and make it reusable.

### a. **Built-in Modules**

Python comes with a set of built-in modules that provide useful functionality. Here are two examples:

#### i. `math` Module

The `math` module provides mathematical functions and constants.

**Example 1: Using `math.sqrt()`**

```python
import math

result = math.sqrt(16)
print("Square Root:", result)
```

**Example 2: Using `math.pi`**

```python
import math

circumference = 2 * math.pi * 5
print("Circumference of a Circle:", circumference)
```

#### ii. `random` Module

The `random` module is used to generate random numbers and perform random operations.

**Example 1: Generating a Random Integer**

```python
import random

random_number = random.randint(1, 10)
print("Random Number:", random_number)
```

**Example 2: Shuffling a List**

```python
import random

my_list = [1, 2, 3, 4, 5]
random.shuffle(my_list)
print("Shuffled List:", my_list)
```

## 2. **Libraries**

Libraries are collections of modules that serve specific purposes or domains, such as web development, data analysis, or machine learning. Users can install and use libraries to leverage their functionality.

### a. **NumPy Library**

NumPy is a popular library for numerical computing in Python. It provides support for arrays and matrices, along with a wide range of mathematical functions.

**Example 1: Creating a NumPy Array**

```python
import numpy as np

my_array = np.array([1, 2, 3, 4, 5])
print("NumPy Array:", my_array)
```

**Example 2: Performing Array Operations**

```python
import numpy as np

array1 = np.array([1, 2, 3])
array2 = np.array([4, 5, 6])
result = array1 + array2
print("Array Addition:", result)
```

### b. **Pandas Library**

The Pandas library is widely used for data manipulation and analysis in Python. It provides data structures like DataFrames for working with structured data.

**Example 1: Creating a DataFrame**

```python
import pandas as pd

data = {'Name': ['Alice', 'Bob', 'Charlie'],
        'Age': [25, 30, 35]}
df = pd.DataFrame(data)
print("DataFrame:\n", df)
```

**Example 2: Reading Data from a CSV File**

```python
import pandas as pd

df = pd.read_csv('data.csv')
print("Read Data:\n", df)
```

Modules and libraries are powerful tools in Python that enhance its capabilities and enable developers to build a wide range of applications efficiently.

## Thank You
- Excited for more ? Subscribe the channel and hit the bell icon to recieve notifications of further contents.

## Next up in the series

- Basics of python continued
    
    + File Management using python


## Contact Me

- Author -- Abhay Kabdwal -- Doctor_Innovator
- **_[Youtube](https://www.youtube.com/@doctor_innovator/featured)_**
- **_[Discord](https://discord.gg/7ydGD3aJ)_**
- **_[Telegram](https://t.me/doctor_innovator)_**