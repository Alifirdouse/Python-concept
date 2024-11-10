# Python Programming Overview

 - Python Basics
 - Data Structures
 - Control Statements
 - Functions
 - Object-Oriented Programming (OOP)
 - File Handling

 # 1. Python Basics
 -----------------
 Python is a high-level, interpreted programming language known for its readability and simplicity. It is dynamically typed, meaning you don't need to declare the type of a variable explicitly.

 Example: Hello 
 
print("Hello, World!")  
 Output: Hello, World!

# 2. Data Structures
 -------------------
 Python provides several built-in data structures such as List, Tuple, Dictionary, and Set.

# List: An ordered, mutable collection of elements.

my_list = [1, 2, 3, 4]

my_list.append(5) 

Adds an element to the list

print(f"List: {my_list}")  
 Output: [1, 2, 3, 4, 5]

# Tuple:An ordered, immutable collection of elements.

my_tuple = (1, 2, 3)

 Tuples cannot be changed after creation, but can be accessed by index.

print(f"Tuple: {my_tuple}")  
Output: (1, 2, 3)

# Dictionary:A collection of key-value pairs, where keys must be unique.

my_dict = {"name": "Alice", "age": 25}
print(f"Dictionary: {my_dict}") 
Output: {'name': 'Alice', 'age': 25}

# Set: An unordered collection of unique elements.

my_set = {1, 2, 3, 4}

my_set.add(5)  
Adding an element to the set

print(f"Set: {my_set}") 
Output: {1, 2, 3, 4, 5}

# 3. Control Statements
#
 -----------------------
#
 Control statements in Python help manage the flow of execution.

# if-else Statement
x = 10
if x > 5:
    print("x is greater than 5")
else:
    print("x is less than or equal to 5")

# for Loop: Used to iterate over a sequence.
for i in range(5):
    print(f"for loop iteration {i}")  # Output: 0, 1, 2, 3, 4

# while Loop: Repeats as long as the condition is true.
x = 0
while x < 3:
    print(f"while loop iteration {x}")  # Output: 0, 1, 2
    x += 1

# 4. Functions
 -------------
# Functions allow you to define reusable blocks of code.

#
 Defining a function

def greet(name):
    return f"Hello, {name}!"

 Calling the function

print(greet("Alice")) 

 Output: Hello, Alice!

# 5. Object-Oriented Programming (OOP)
 -------------------------------------
 Python supports OOP, where you bundle data and methods into objects.

 Defining a class

class Dog:

    def __init__(self, name, age):
        self.name = name
        self.age = age

    def bark(self):
        return f"{self.name} says Woof!"

# Creating an object (instance of the class)
my_dog = Dog("Buddy", 3)

print(my_dog.bark())  # Output: Buddy says Woof!

# Inheritance:
 Allows one class to inherit from another.

class Animal:
    def speak(self):
        return "Animal speaks"

class Dog(Animal):
    def speak(self):
        return "Woof!"

my_dog = Dog()
print(my_dog.speak())  # Output: Woof!

# 6. File Handling
 -----------------
 Python provides built-in functions to read from and write to files.

# Writing to a file
with open("example.txt", "w") as file:
    file.write("Hello, World!")
    file.write("\nAppended text")

# Reading from a file
with open("example.txt", "r") as file:

    content = file.read()
    print(f"File Content: {content}")  # Output: Hello, World!\nAppended text

# Appending to a file
with open("example.txt", "a") as file:

    file.write("\nAnother line appended")

# Reading updated file content
with open("example.txt", "r") as file:

    content = file.read()
    print(f"Updated File Content: {content}")  # Output: Hello, World!\nAppended text\nAnother line appended

