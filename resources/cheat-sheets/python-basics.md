# Python Basics Cheat Sheet

## 📌 Quick Reference for Python Beginners

### Comments
```python
# Single-line comment

"""
Multi-line comment
(also called docstring)
"""
```

### Output
```python
print("Hello")              # Print text
print(42)                   # Print number
print("Hello", "World")     # Print multiple items
print("Age:", 25)           # Mix text and numbers
```

### Variables
```python
name = "Alice"              # String variable
age = 25                    # Integer variable
height = 5.6                # Float variable
is_student = True           # Boolean variable
```

### Data Types
```python
# String (text)
text = "Hello"
text = 'Hello'              # Single or double quotes

# Integer (whole numbers)
count = 10
negative = -5

# Float (decimal numbers)
price = 19.99
temperature = -3.5

# Boolean (True/False)
is_valid = True
is_complete = False
```

### Basic Operations
```python
# Arithmetic
5 + 3        # Addition: 8
10 - 4       # Subtraction: 6
3 * 4        # Multiplication: 12
15 / 3       # Division: 5.0
15 // 3      # Integer division: 5
17 % 5       # Modulus (remainder): 2
2 ** 3       # Exponentiation: 8

# String operations
"Hello" + "World"           # Concatenation: "HelloWorld"
"Hi" * 3                    # Repetition: "HiHiHi"
len("Hello")                # Length: 5
```

### Input
```python
name = input("Enter name: ")           # Get user input (string)
age = int(input("Enter age: "))        # Convert to integer
price = float(input("Enter price: "))  # Convert to float
```

### Conditionals
```python
# If statement
if age >= 18:
    print("Adult")

# If-else
if age >= 18:
    print("Adult")
else:
    print("Minor")

# If-elif-else
if grade >= 90:
    print("A")
elif grade >= 80:
    print("B")
elif grade >= 70:
    print("C")
else:
    print("F")
```

### Comparison Operators
```python
==    # Equal to
!=    # Not equal to
>     # Greater than
<     # Less than
>=    # Greater than or equal to
<=    # Less than or equal to
```

### Logical Operators
```python
and   # Both conditions must be True
or    # At least one condition must be True
not   # Inverts the condition

# Examples
age >= 18 and age < 65
is_weekend or is_holiday
not is_raining
```

### Loops
```python
# While loop
count = 0
while count < 5:
    print(count)
    count += 1

# For loop with range
for i in range(5):          # 0, 1, 2, 3, 4
    print(i)

for i in range(1, 6):       # 1, 2, 3, 4, 5
    print(i)

for i in range(0, 10, 2):   # 0, 2, 4, 6, 8
    print(i)
```

### Lists
```python
# Creating lists
fruits = ["apple", "banana", "cherry"]
numbers = [1, 2, 3, 4, 5]
mixed = [1, "two", 3.0, True]

# Accessing elements
fruits[0]           # First element: "apple"
fruits[-1]          # Last element: "cherry"

# List operations
fruits.append("date")       # Add to end
fruits.insert(1, "blueberry")  # Insert at position
fruits.remove("banana")     # Remove by value
fruits.pop()                # Remove last element
len(fruits)                 # Length of list

# Looping through lists
for fruit in fruits:
    print(fruit)
```

### Strings
```python
text = "Hello World"

# String methods
text.lower()        # "hello world"
text.upper()        # "HELLO WORLD"
text.strip()        # Remove whitespace
text.split()        # ["Hello", "World"]
text.replace("World", "Python")  # "Hello Python"

# String indexing and slicing
text[0]             # "H"
text[-1]            # "d"
text[0:5]           # "Hello"
text[6:]            # "World"
```

### Functions
```python
# Defining a function
def greet(name):
    return f"Hello, {name}!"

# Calling a function
message = greet("Alice")
print(message)

# Function with multiple parameters
def add(a, b):
    return a + b

result = add(5, 3)

# Function with default parameter
def greet(name="Guest"):
    return f"Hello, {name}!"
```

### String Formatting
```python
name = "Alice"
age = 25

# f-strings (Python 3.6+)
print(f"Name: {name}, Age: {age}")

# format method
print("Name: {}, Age: {}".format(name, age))

# % operator (old style)
print("Name: %s, Age: %d" % (name, age))
```

### Dictionaries
```python
# Creating a dictionary
person = {
    "name": "Alice",
    "age": 25,
    "city": "New York"
}

# Accessing values
print(person["name"])
print(person.get("age"))

# Adding/updating entries
person["email"] = "alice@example.com"
person["age"] = 26

# Looping through dictionary
for key, value in person.items():
    print(f"{key}: {value}")
```

### Common Built-in Functions
```python
len(item)           # Length
type(item)          # Data type
str(item)           # Convert to string
int(item)           # Convert to integer
float(item)         # Convert to float
max(list)           # Maximum value
min(list)           # Minimum value
sum(list)           # Sum of values
range(start, stop, step)  # Generate sequence
```

### File Operations
```python
# Reading a file
with open("file.txt", "r") as file:
    content = file.read()

# Writing to a file
with open("file.txt", "w") as file:
    file.write("Hello, World!")

# Appending to a file
with open("file.txt", "a") as file:
    file.write("More text")
```

### Error Handling
```python
try:
    result = 10 / 0
except ZeroDivisionError:
    print("Cannot divide by zero!")
except Exception as e:
    print(f"An error occurred: {e}")
finally:
    print("This always executes")
```

### Useful Tips
```python
# Multiple assignment
x, y, z = 1, 2, 3

# Swap variables
a, b = b, a

# Check if item in list
if "apple" in fruits:
    print("Found!")

# Ternary operator
status = "Adult" if age >= 18 else "Minor"

# List comprehension
squares = [x**2 for x in range(10)]
```

---

## 💡 Remember
- Python is case-sensitive: `Print` ≠ `print`
- Indentation matters: Use 4 spaces for blocks
- Use meaningful variable names
- Comment your code
- Test frequently
- Practice regularly!

---

Happy coding! 🐍
