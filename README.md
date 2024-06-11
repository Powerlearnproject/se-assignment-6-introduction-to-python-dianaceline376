[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15256159&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

      ANSWER:
      -------
1. ## Python Basics

### What is Python, and What Are Some of Its Key Features?

Python is a high-level, interpreted programming language known for its readability and simplicity. Created by Guido van Rossum and first released in 1991, Python has become one of the most popular programming languages in the world.

#### Key Features:
- **Readable Syntax**: Python's syntax is clean and easy to understand, making it accessible to beginners.
- **Interpreted Language**: Python code is executed line by line, which makes debugging easier.
- **Dynamically Typed**: Variables in Python do not need explicit declaration to reserve memory space.
- **Extensive Standard Library**: Python comes with a large standard library that supports many common programming tasks.
- **Cross-Platform**: Python can run on various operating systems like Windows, macOS, and Linux.
- **Community Support**: Python has a large, active community, which contributes to a rich ecosystem of third-party libraries and frameworks.

#### Use Cases:
- **Web Development**: Using frameworks like Django and Flask.
- **Data Analysis and Visualization**: Libraries like pandas, NumPy, and Matplotlib.
- **Machine Learning and AI**: Libraries like TensorFlow, Keras, and scikit-learn.
- **Automation and Scripting**: Automating repetitive tasks and system administration.
- **Scientific Computing**: Libraries like SciPy.

2. ## Installing Python

### Steps to Install Python (Windows Example):

i. **Download Python**:
   - Visit the official [Python website](https://www.python.org/).
   - Download the latest Python installer for Windows.

ii. **Run the Installer**:
   - Double-click the downloaded installer file.
   - Check the box "Add Python to PATH".
   - Click "Install Now".

iii. **Verify the Installation**:
   - Open Command Prompt (cmd).
   - Type `python --version` or `python -V` to verify the installation.

iv. **Set Up a Virtual Environment**:
   - Open Command Prompt.
   - Navigate to your project directory.
   - Run `python -m venv myenv` to create a virtual environment.
   - Activate the virtual environment:
     - Windows: `myenv\Scripts\activate`
     - macOS/Linux: `source myenv/bin/activate`

3. ## Python Syntax and Semantics

### Simple Python Program

```python
print("Hello, World!")
```

#### Explanation:
- `print`: A built-in function to output text to the console.
- `"Hello, World!"`: A string literal enclosed in double quotes.

4. ## Data Types and Variables

### Basic Data Types
- **int**: Integer numbers.
- **float**: Floating-point numbers.
- **str**: Strings.
- **bool**: Boolean values (`True` or `False`).
- **list**: Ordered, mutable collections.
- **tuple**: Ordered, immutable collections.
- **dict**: Unordered, mutable collections of key-value pairs.
- **set**: Unordered collections of unique elements.

### Example Script
```python
# Integer
num = 10
print(num, type(num))

# Float
pi = 3.14
print(pi, type(pi))

# String
name = "Python"
print(name, type(name))

# Boolean
is_active = True
print(is_active, type(is_active))

# List
fruits = ["apple", "banana", "cherry"]
print(fruits, type(fruits))

# Tuple
coordinates = (10, 20)
print(coordinates, type(coordinates))

# Dictionary
student = {"name": "John", "age": 21}
print(student, type(student))

# Set
unique_numbers = {1, 2, 3, 4, 4, 5}
print(unique_numbers, type(unique_numbers))
```

5. ## Control Structures

### Conditional Statements

```python
age = 18
if age >= 18:
    print("You are an adult.")
else:
    print("You are a minor.")
```

### Loops

#### For Loop

```python
numbers = [1, 2, 3, 4, 5]
for number in numbers:
    print(number)
```

#### While Loop

```python
count = 0
while count < 5:
    print(count)
    count += 1
```

6. ## Functions in Python

### What Are Functions and Why Are They Useful?

Functions are reusable blocks of code that perform a specific task. They help in organizing code, making it more readable and maintainable.

### Example Function

```python
def add(a, b):
    return a + b

# Calling the function
result = add(3, 5)
print(result)
```

7. ## Lists and Dictionaries

### Differences
- **List**: An ordered collection of elements that can be accessed by index.
- **Dictionary**: An unordered collection of key-value pairs where keys are unique.

### Example Script

```python
# List
numbers = [1, 2, 3, 4, 5]
numbers.append(6)
print(numbers)
print(numbers[2])

# Dictionary
student = {"name": "Alice", "age": 25}
student["grade"] = "A"
print(student)
print(student["name"])
```

8. ## Exception Handling

### What Is Exception Handling?

Exception handling is a way to handle errors gracefully in a program using `try`, `except`, and `finally` blocks.

### Example

```python
try:
    result = 10 / 0
except ZeroDivisionError as e:
    print("Error:", e)
finally:
    print("This will always execute.")
```

9. ## Modules and Packages

### Concepts

- **Module**: A file containing Python code (functions, classes, variables) that can be imported and used in other Python programs.
- **Package**: A collection of related modules.

### Example Using the Math Module

```python
import math

print(math.sqrt(16))  # 4.0
print(math.pi)        # 3.141592653589793
```

10. ## File I/O

### Reading and Writing Files

#### Reading from a File

```python
with open('example.txt', 'r') as file:
    content = file.read()
    print(content)
```

#### Writing to a File

```python
lines = ["First line", "Second line", "Third line"]
with open('output.txt', 'w') as file:
    for line in lines:
        file.write(line + "\n")
```



# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


