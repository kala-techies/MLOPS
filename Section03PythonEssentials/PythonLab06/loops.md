
# PythonLab06: Loops

## Overview
This module introduces loop constructs in Python, providing the foundation for iterating through sequences, managing conditions, and controlling flow within loops. Mastering loops will enable you to execute code multiple times effectively and streamline repetitive tasks in your programs.

## Table of Contents
1. [Introduction to Loops](#introduction-to-loops)
2. [The `for` Loop](#the-for-loop)
    - [Iterating Over a Range](#iterating-over-a-range)
    - [Iterating Over a String](#iterating-over-a-string)
3. [The `while` Loop](#the-while-loop)
4. [Loop Control Statements](#loop-control-statements)
    - [`break` Statement](#break-statement)
    - [`continue` Statement](#continue-statement)
    - [`pass` Statement](#pass-statement)
5. [Nested Loops](#nested-loops)
6. [Conclusion](#conclusion)

## Introduction to Loops
Loops are an essential feature in Python, allowing you to repeat a block of code multiple times. They are particularly useful when working with collections, iterating through ranges, or executing code under certain conditions.

## The `for` Loop
The `for` loop is used to iterate over a sequence (like a list, tuple, string, or range). It provides a convenient way to repeat actions with minimal code.

### Iterating Over a Range
Use `range()` to create a sequence of numbers to iterate over:
```python
for i in range(5):
    print(i)
```

### Iterating Over a String
Strings can also be iterated character by character:
```python
for char in "Python":
    print(char)
```

## The `while` Loop
The `while` loop runs as long as a specified condition remains `True`. It is particularly useful for cases where the number of iterations depends on dynamic conditions.
```python
count = 0
while count < 5:
    print(count)
    count += 1
```

## Loop Control Statements
Loop control statements allow for more flexible loop execution by modifying the loop's behavior based on specific conditions.

### `break` Statement
The `break` statement exits the loop prematurely, terminating the loop when a specified condition is met.
```python
for i in range(10):
    if i == 5:
        break
    print(i)
```

### `continue` Statement
The `continue` statement skips the current iteration and moves to the next one.
```python
for i in range(5):
    if i == 2:
        continue
    print(i)
```

### `pass` Statement
The `pass` statement does nothing. It’s a placeholder often used as a temporary code structure while developing.
```python
for i in range(5):
    if i == 3:
        pass  # Placeholder for future code
    print(i)
```

## Nested Loops
A nested loop is a loop within another loop. Nested loops are helpful for working with multi-dimensional data structures.
```python
for i in range(3):
    for j in range(2):
        print(f"i: {i}, j: {j}")
```

## Conclusion
Loops are powerful tools in Python that simplify repetitive tasks by allowing code to execute multiple times efficiently. By mastering `for` and `while` loops, along with control statements like `break`, `continue`, and `pass`, you can write more effective and concise programs.

---