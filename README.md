# Complete Introduction to Python

## What is Python and Why Learn It?
Python is a general-purpose programming language designed to be easy to read and write. It was created in 1991 by Guido van Rossum with the goal of helping developers write readable code, maintain large projects, and solve problems efficiently.

### Why Learn Python?
Python is recognized as one of the most versatile and in-demand languages. Learning it offers key benefits:

- **Ease of Use**:
  - Its syntax is similar to human language, making it perfect for beginners.
  - Compared to languages like C++ or Java, Python requires fewer lines to achieve the same result.
  
- **Practical Applications**:
  - **Automation**: Create scripts to perform repetitive tasks (e.g., moving files, generating reports, etc.).
  - **Data Science and Machine Learning**: Libraries like pandas, NumPy, and TensorFlow make Python the standard for data analysis and prediction.
  - **Web Development**: Frameworks like Django and Flask are used to build robust, scalable web applications.
  - **Rapid Prototyping**: Its speed of development allows quick prototyping of concepts.
  
- **High Job Demand**: Python is one of the most requested languages in the job market, especially in emerging fields like AI, software development, and data science.

### Who Can Learn Python?
Python is ideal for both beginners and experienced developers. You can learn it if:

- You want to take your first steps in programming.
- You work in fields like data analysis, finance, biology, or engineering.
- You wish to automate daily tasks.

## Setting Up Your Development Environment

### What Do You Need to Get Started?
Before you start writing Python code, you need:

1. **Install Python on your computer**.
2. **Choose a text editor or development environment (IDE)**.
3. **Verify that everything works correctly**.

### Step 1: Installing Python

- **Windows/MacOS**:
  - Download Python from [python.org](https://www.python.org).
  - Ensure you select "Add Python to PATH" during the installation process. This allows Python to be used from any terminal.

- **Linux**: Python is typically pre-installed. To check the version, run:
  
  ```bash
  python3 --version
  ```
If it's not installed, use:

```bash
sudo apt update
sudo apt install python3
```

Step 2: Install a Code Editor

A good text editor helps write and debug code more easily. Recommended editors:

Visual Studio Code:

- Lightweight, intuitive, and with extensions like Python to run and debug code easily.

- Download from VS Code.

- Install the "Python" extension from the extensions section.
  
Step 3: Verify Installation

Open a terminal and type:

```bash
python3 --version
```
You should see the installed version number.

First Execution
Test that everything works by creating a file called hello.py:

```python
print("Hello, World")
```

Run this file from the terminal with:

```bash
python3 hello.py
```

You should see:

```bash
Hello, World
```
Comments in Python

What are Comments?

Comments are lines of text within the code that are ignored by the interpreter. They are used to explain the code and make it easier to understand, especially when:

Collaborating with other developers

Remembering why certain decisions were made

Types of Comments
Single-line comment: Starts with the # symbol.
```python
# This is a comment
print("Hello, World")  # This comment explains what this line does
```
Multi-line comment: Uses triple quotes (''' or """).

```python
"""
This is a comment
that spans multiple lines.
Used for extensive explanations.
"""
```
Data Types in Python

What are Data Types?

Data in Python can be classified into different types, depending on the value they represent. Data types are important because they:

Determine how values can be manipulated or processed.
Enable specific validations or calculations.

Basic Data Types
Integers (int): Represent whole numbers.

Common uses:

Counting items.
Performing mathematical operations.
Example:

```python
age = 25
print(age + 5)  # 30
```
- Floating-point numbers (float): Represent numbers with decimals.

   - Common uses:

- Working with prices, measurements, or percentages.

   - Example:

```python
temperature = 36.6
print(temperature * 2)  # 73.2
```
Strings (str): Represent text. Can include words, phrases, numbers as text, or special characters.

Common uses:

- Storing names, messages, or visual information.

   - Example:

```python
greeting = "Hello"
name = "Ana"
print(greeting + " " + name)  # Hello Ana
```
Booleans (bool): Represent truth values: True or False.

Common uses:

Logical decisions (if, while, etc.).
Example:

```python
is_adult = True
print(is_adult)  # True
```
Complex numbers (complex): Include both a real and imaginary part

Common uses:

- Mathematical and scientific applications.
   - Example:

```python
complex_number = 3 + 4j
print(complex_number.real)  # 3.0
print(complex_number.imag)  # 4.0
```

How to Identify the Data Type?

Use the type() function:

```python
data = 42
print(type(data))  # <class 'int'>
```

Variables in Python

What are Variables?

Variables are containers that store values. They can change their content during the program's execution.

Characteristics of Variables in Python

No need to declare the type: Python automatically detects the type based on the assigned value.
They can change their value:

```python
x = 10
print(x)  # 10
x = 20
print(x)  # 20
```
Best Practices
Use descriptive names:

```python
user_age = 30  # Good
x = 30  # Not recommended
```
Follow the snake_case format:

```python
full_name = "Carlos Pérez"
Multiple Declarations
```

You can assign multiple values at once:

```python
a, b, c = 10, 20, 30
print(a, b, c)  # 10 20 30
```

# Variables in Python

## What is a variable?

A variable is a name associated with a value that you can use and modify during the execution of a program. It's like a "box" where you store data to use later.

### Why are variables important?
- **Data reuse**: Once a value is assigned to a variable, you can use it as many times as needed

- **Flexibility**: The content of a variable can change dynamically based on the program's needs

- **Readability**: Descriptive names make the code easier to understand

### How to declare and use variables
To declare a variable, simply write its name and assign it a value using the `=` operator:

```python
age = 25
name = "Carlos"
is_adult = True
```
After declaration, you can use variables in operations, conditionals, or functions:

```python
print("The user's name is:", name)  # Output: The user's name is: Carlos
print("Is the user an adult?", is_adult)  # Output: Is the user an adult? True
```
Variable overwriting

The value of a variable can change during the program:

```python
x = 5
print(x)  # 5
x = 10
print(x)  # 10
```
Rules for naming variables

They must start with a letter or an underscore (_), but never with a number
They cannot contain spaces. Use underscores instead:

```python
user_name = "Ana"  # Correct
user name = "Ana"  # Incorrect
```
You cannot use reserved words like if, else, True, etc

They are case-sensitive:

```python
Age = 25  # Different from age
```

Variable types

- Variables in Python can store any type of data. 
  - Example:

```python
integer = 42
floating_point = 3.14
string = "Hello"
boolean = False
```

Multiple assignment

You can assign multiple values in one line:

```python
a, b, c = 1, 2, 3
print(a, b, c)  # 1 2 3
```
Best practices when using variables

Use descriptive names to make the code easier to read:

```python
car_speed = 120  # Clear and understandable
v = 120  # Not very clear
```
Follow the snake_case format for names:

```python
full_name = "Carlos Pérez"
```
If the variable is a constant, use uppercase letters:

```python
PI = 3.14159
```

## Data Structures

What are data structures?

Data structures allow you to store and organize collections of data efficiently. In Python, the main ones are:

- Lists: Ordered and mutable collections
- Tuples: Ordered and immutable collections
- Dictionaries: Unordered collections of key-value pairs
- Sets: Unordered collections of unique elements

1. Lists
What are lists?

A list is an ordered collection that allows you to store multiple elements in a single variable. Lists are mutable, meaning you can change their content after creation.

What are lists used for?
Storing groups of related elements (names, numbers, results).
Performing operations like sorting, searching, or deleting data.
Basic syntax

```python
fruits = ["apple", "banana", "cherry"]
```

Accessing elements

Use indices to access elements in a list. Remember that indices start at 0

```python
print(fruits[0])  # apple
print(fruits[2])  # cherry
```

Common operations
Adding elements:

```python
fruits.append("pear")
print(fruits)  # ['apple', 'banana', 'cherry', 'pear']
```
Removing elements:

```python
fruits.remove("banana")
print(fruits)  # ['apple', 'cherry']
```
Getting the size of the list:

```python
print(len(fruits))  # 2
```

Iterating over a list:

```python
for fruit in fruits:
    print(fruit)
```
Sorting the list:

```python
fruits.sort()
print(fruits)  # ['cherry', 'apple']
```
2. Tuples
What are tuples?

Tuples are similar to lists but are immutable (you cannot change their content after creation)

What are tuples used for?

Storing data that should not change (coordinates, settings)

Using them as keys in dictionaries since they are immutable

Basic syntax

```python
colors = ("red", "green", "blue")
```
Accessing elements

Just like with lists, use indices:

```python
print(colors[1])  # green
Common operations
```
Even though you can't modify tuples, you can:

Count elements:

```python
print(colors.count("red"))  # 1
```

Get the index of an element:

```python
print(colors.index("blue"))  # 2
```
3. Dictionaries
   
What are dictionaries?

A dictionary stores key-value pairs, where each key is unique

What are dictionaries used for?

Modeling relationships between data, like names and phone numbers
Quickly accessing values using keys

Basic syntax

```python
person = {"name": "Ana", "age": 25}
```
Accessing elements
Use the key to get the value:

```python
print(person["name"])  # Ana
```
Common operations
Adding a key-value pair:

```python
person["city"] = "Madrid"
```
Removing a key:
```python
del person["age"]
```
Iterating over keys and values:
```python
for key, value in person.items():
    print(key, value)
```
4. Sets
What are sets?
Sets are unordered collections of unique elements.

What are sets used for?

Removing duplicates from a collection
Performing mathematical operations like intersection or union

Basic syntax

```python
numbers = {1, 2, 3, 3}
print(numbers)  # {1, 2, 3}
```
Common operations

Adding elements:

```python
numbers.add(4)
```
Intersection with another set:

```python
evens = {2, 4, 6}
print(numbers.intersection(evens))  # {2, 4}
```
Union of sets:
```python
print(numbers.union(evens))  # {1, 2, 3, 4, 6}
```
