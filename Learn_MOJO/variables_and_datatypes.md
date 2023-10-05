# Mojo Programming Language: Variables and Data Types

## 1. Variables
In Mojo, you can assign a value to a name inside a `fn`, and it implicitly creates a function scope variable just like in Python. For example:

```mojo
fn main():
    let x = 10
    print(x)  # prints: 10
```
In the above example, `x` is a variable that holds the value `10`. The `let` keyword is used to declare a variable in Mojo.

Mojo also has another type of variable declaration which uses the `var` keyword.
```mojo
fn main():
    var x = 10
    print(x)   # prints: 10
```

On running the above code segment we get a warning and the desired output
```bash
warning: 'x' was declared as a 'var' but never mutated, consider switching to a 'let'
    var x = 10
    ^
10
```

From the above it is clear that the `var` keyword is mutable and the warning says that it is initialized as var but never mutated

Similarly if we try to mutate a variable which is initialized using `let` keyword we get an error.

```mojo
fn main():
    let x = 10
    x = x + 5
    print(x)
```
```bash
error: expression must be mutable in assignment
    x = x + 5
    ^
```

This shows us that the `let` initialization is immutable while the `var` initialization is mutable.

## 2. Data Types
Mojo supports common data types such as integers, floats, strings, and booleans. Additionally, it provides advanced data types like arrays and dictionaries to handle collections of data.

### 2.1 Integer
An integer is a whole number that can be either greater than 0, called positive or less than 0, called negative. Zero is neither positive nor negative. For example:

```mojo
fn main():
    let number = 42  # integer
    print(number)    # prints: 42
```
#### Or
```mojo
fn main():
    let marks: Int = 91                 # integer
    print("Your marks are :",marks)     # prints: Your marks are 91
```

### 2.2 Float
A floating point number is a number, positive or negative, containing one or more decimals. For example:

```mojo
fn main():
    let pi = 3.14     # float
    print(pi)         # prints: 3.14
```
#### Or
```mojo
fn main():
    let score: Float64 = 8.2              # float
    print("Your score is :", score)       # prints: Your score is 8.2
```

### 2.3 String
Strings in Mojo are surrounded by either single quotation marks, or double quotation marks. For example:

```mojo
fn main():
    let name = "Mojo"    # string
    print(name)          # prints: Mojo
```
#### Or
```mojo
fn main():
    let language: String = "Mojo"       # string
    print(language + " is awesome")     # prints: Mojo is awesome
    print(language,"is awesome")
``` 
### 2.4 Boolean
Booleans represent one of two values: `true` or `false`. For example:

```mojo
fn main():
    let is_true = true    # boolean
    print(is_true)        # prints: true
```

#### Or
```mojo
fn main():
    let is_false: Bool = false      # boolean
    print(is_false)                 # prints: false
```
## Thank You
- Excited for more ? Subscribe the channel and hit the bell icon to recieve notifications of further contents. Also join my discord server and telegram channel for updates and resources.

## Contact Me

- Author -- Abhay Kabdwal -- Doctor_Innovator
- **_[Youtube](https://www.youtube.com/@doctor_innovator/featured)_**
- **_[Discord](https://discord.gg/7ydGD3aJ)_**
- **_[Telegram](https://t.me/doctor_innovator)_**