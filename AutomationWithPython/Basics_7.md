# Basics of File Management in Python

File management in Python is essential for reading, writing, and manipulating files. This markdown script outlines the fundamental concepts and operations related to file management, along with examples for each.

## Table of Contents
1. [Opening and Closing Files](#1-opening-and-closing-files)
2. [Reading Files](#2-reading-files)
3. [Writing Files](#3-writing-files)
4. [File Modes](#4-file-modes)
5. [Working with Text Files](#5-working-with-text-files)
6. [Working with Binary Files](#6-working-with-binary-files)
7. [File Handling using `with` Statement](#7-file-handling-using-with-statement)
8. [File Navigation and Location](#8-file-navigation-and-location)
9. [File Information](#9-file-information)

---

### 1. Opening and Closing Files
To work with files in Python, you must first open them and close them when you're done.

#### Example : Opening and Closing a Text File
```python
# Open a file in write mode
file = open('example.txt', 'w')
# ... do some operations ...
file.close()  # Close the file when done
```

#### Example : Opening and Closing a Binary File
```python
# Open a binary file in read mode
binary_file = open('data.bin', 'rb')
# ... do some operations ...
binary_file.close()  # Close the binary file
```

### 2. Reading Files
Reading data from files is a common task in Python.

#### Example : Reading a Text File Line by Line
```python
with open('example.txt', 'r') as file:
    for line in file:
        print(line.strip())  # Strip newline character
```

#### Example : Reading the Entire Contents of a Binary File
```python
with open('data.bin', 'rb') as binary_file:
    data = binary_file.read()
    # Process binary data here
```

### 3. Writing Files
You can write data to files using various methods.

#### Example : Writing to a Text File
```python
with open('example.txt', 'w') as file:
    file.write('Hello, World!\n')
    file.write('Python is awesome!')
```

#### Example : Writing to a Binary File
```python
with open('data.bin', 'wb') as binary_file:
    binary_data = bytes([0x48, 0x65, 0x6C, 0x6C, 0x6F])
    binary_file.write(binary_data)
```

### 4. File Modes
Python supports different file modes for opening files.

- `'r'`: Read (default)
- `'w'`: Write
- `'a'`: Append
- `'b'`: Binary
- `'t'`: Text (default)

### 5. Working with Text Files
Text files store data in a human-readable format.

#### Example : Reading and Writing Text Files
```python
with open('textfile.txt', 'w') as text_file:
    text_file.write('Python is fun!')

with open('textfile.txt', 'r') as text_file:
    content = text_file.read()
    print(content)
```

### 6. Working with Binary Files
Binary files store data in a non-human-readable format.

#### Example 1: Reading and Writing Binary Files
```python
with open('binaryfile.bin', 'wb') as binary_file:
    binary_data = bytes([0x48, 0x65, 0x6C, 0x6C, 0x6F])
    binary_file.write(binary_data)

with open('binaryfile.bin', 'rb') as binary_file:
    data = binary_file.read()
    # Process binary data here
```

### 7. File Handling using `with` Statement
Using the `with` statement is recommended because it automatically closes files.

### 8. File Navigation and Location
Python provides methods for navigating and locating files.

#### Example 1: Checking File Existence
```python
import os

if os.path.exists('myfile.txt'):
    print('File exists!')
else:
    print('File does not exist.')
```

#### Example 2: Listing Files in a Directory
```python
import os

files_in_directory = os.listdir('.')
for file_name in files_in_directory:
    print(file_name)
```

### 9. File Information
You can obtain information about files, such as size and modification time.

#### Example 1: Getting File Size and Modification Time
```python
import os

file_info = os.stat('myfile.txt')
print(f'File Size: {file_info.st_size} bytes')
print(f'Modification Time: {file_info.st_mtime}')
```

These basics of file management in Python should provide a solid foundation for working with files in your Python programs.