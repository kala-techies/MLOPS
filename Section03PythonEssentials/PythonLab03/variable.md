
# Lab 3: Introduction to Variables in Python

This lab introduces the concept of variables in Python, including how to declare, assign, and manipulate them. We'll cover variable naming conventions, types, type checking and conversion, dynamic typing, and user input.

## Table of Contents
1. [Introduction to Variables](#introduction-to-variables)
2. [Declaring and Assigning Variables](#declaring-and-assigning-variables)
3. [Naming Conventions](#naming-conventions)
4. [Understanding Variable Types](#understanding-variable-types)
5. [Type Checking and Conversion](#type-checking-and-conversion)
6. [Dynamic Typing](#dynamic-typing)
7. [User Input](#user-input)

---

### Introduction to Variables

Variables are fundamental elements in programming used to store data that can be referenced and manipulated in a program. In Python, variables are created when you assign a value to them. Python’s memory management allocates the necessary space automatically, so you don’t need to explicitly declare variables before using them.

### Declaring and Assigning Variables

Variables are declared and assigned values using the assignment operator `=`. For example:
```python
first_name = "kala"
age = 25
```

### Naming Conventions

In Python, there are specific conventions and rules for naming variables:
- **Descriptive Names**: Variable names should be descriptive, representing the data they hold.
- **Start with a Letter or Underscore**: Variable names must start with a letter (a-z, A-Z) or an underscore (_).
- **Case Sensitivity**: Variable names are case-sensitive, meaning `Name` and `name` are treated as two different variables.

Examples:
```python
# Valid variable names
first_name = "kala"
last_name = "techies"

# Invalid variable names
2firstname = "kala"    # Starts with a number
first-name = "joy"     # Contains a hyphen
```

### Understanding Variable Types

Python is a dynamically typed language, meaning the type of a variable is determined at runtime. The type is based on the value assigned to the variable:
```python
age = 25          # Integer
name = "kala"     # String
height = 5.9      # Float
```

### Type Checking and Conversion

Python allows you to check a variable's type using `type()`. It also supports type conversion, or casting, to change a variable's data type.

Examples:
```python
age = 25
print(type(age))       # Output: <class 'int'>

# Type Conversion
age_str = str(age)     # Converts integer to string
print(age_str)         # Output: "25"
print(type(age_str))   # Output: <class 'str'>

# Converting float to string and vice versa is possible:
height = 5.9
height_str = str(height)   # Converts float to string

# Converting a complete string to int may not be possible without a numeric value:
# e.g., int("abc") would cause an error
```

### Dynamic Typing

One of Python’s standout features is its dynamic typing, which allows variables to change type at runtime. This provides flexibility but can also lead to unexpected behavior if not managed carefully.

Example:
```python
var = 10
print(var, type(var))   # Output: 10 <class 'int'>

var = "hello"
print(var, type(var))   # Output: hello <class 'str'>
```

### User Input

Python can capture user input using the `input()` function. By default, `input()` returns the input as a string, so type conversion may be necessary if a specific data type is required.

Examples:
1. Basic input:
    ```python
    age = input("What is your age? ")
    print(age)
    ```

2. Checking input type:
    ```python
    age = input("What is your age? ")
    print(age, type(age))   # Output will be <class 'str'>
    ```

3. Type casting input:
    ```python
    age = int(input("What is your age? "))  # Type cast from str to int
    print(age, type(age))   # Output will be <class 'int'>
    ```

---

This lab provides a foundational understanding of variables in Python, setting the stage for more advanced programming concepts. For further exploration, see Python’s [official documentation](https://docs.python.org/3/) on variables.