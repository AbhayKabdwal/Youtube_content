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

- Author -- Abhay Kabdwal -- Doctor_Innovator
- **_[Youtube](https://www.youtube.com/@doctor_innovator/featured)_**
- **_[Discord](https://discord.gg/7ydGD3aJ)_**
- **_[Telegram](https://t.me/doctor_innovator)_**