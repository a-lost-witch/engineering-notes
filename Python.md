## 1. What is a Variable?

### Answer:
A variable is a named storage location used to store data in a program. The value of a variable can change during program execution.

### Example:
```python
name = "Adrita"
age = 22
```

---

## 2. What are Data Types in Python?

### Answer:
Data types define the type of data that can be stored in a variable.

Common data types:
- int (Integer)
- float (Decimal Number)
- str (String)
- bool (Boolean)
- list
- tuple
- set
- dict

### Example:
```python
age = 22          # int
salary = 35000.5 # float
name = "Adrita"  # str
is_active = True # bool
```

---

## 3. What is a Function?

### Answer:
A function is a block of reusable code that performs a specific task.

### Example:
```python
def greet(name):
    return f"Hello, {name}"

print(greet("Adrita"))
```

### Output:
```
Hello, Adrita
```

---

## 4. Why are Functions Used?

### Answer:
Functions help:
- Reuse code
- Reduce duplication
- Improve readability
- Simplify maintenance

### Example:
```python
def add(a, b):
    return a + b

print(add(10, 20))
```

---

## 5. What is a Loop?

### Answer:
A loop is used to execute a block of code repeatedly.

Types of loops:
- for loop
- while loop

### Example:
```python
for i in range(5):
    print(i)
```

### Output:
```
0
1
2
3
4
```

---

## 6. What is a for Loop?

### Answer:
A for loop iterates over a sequence such as a list, tuple, string, or range.

### Example:
```python
fruits = ["Apple", "Banana", "Mango"]

for fruit in fruits:
    print(fruit)
```

---

## 7. What is a while Loop?

### Answer:
A while loop executes as long as a condition remains True.

### Example:
```python
count = 1

while count <= 5:
    print(count)
    count += 1
```

---

## 8. What is a Class?

### Answer:
A class is a blueprint for creating objects. It defines properties (attributes) and behaviors (methods).

### Example:
```python
class Student:
    def __init__(self, name):
        self.name = name

student1 = Student("Adrita")
print(student1.name)
```

### Output:
```
Adrita
```

---

## 9. What is an Object?

### Answer:
An object is an instance of a class.

### Example:
```python
class Car:
    pass

car1 = Car()
```

Here:
- Car → Class
- car1 → Object

---

## 10. What is the __init__ Method?

### Answer:
The __init__ method is a constructor that runs automatically when an object is created.

### Example:
```python
class Employee:
    def __init__(self, name):
        self.name = name

emp = Employee("John")
```

---

## 11. What is File Handling?

### Answer:
File handling is the process of creating, reading, writing, and modifying files.

Common modes:
- r → Read
- w → Write
- a → Append
- x → Create

---

## 12. How to Read a File?

### Example:
```python
file = open("sample.txt", "r")
content = file.read()
print(content)
file.close()
```

---

## 13. How to Write to a File?

### Example:
```python
file = open("sample.txt", "w")
file.write("Hello World")
file.close()
```

---

## 14. What is the Difference Between 'w' and 'a' Mode?

### Answer:

| Mode | Description |
|--------|------------|
| w | Overwrites existing content |
| a | Adds content at the end |

### Example:
```python
file = open("sample.txt", "a")
file.write("New Line")
file.close()
```

---

## 15. What is a Dictionary?

### Answer:
A dictionary stores data in key-value pairs.

### Example:
```python
student = {
    "name": "Adrita",
    "age": 22,
    "city": "Kolkata"
}

print(student["name"])
```

### Output:
```
Adrita
```

---

## 16. What is a Key-Value Pair?

### Answer:
A key-value pair consists of:
- Key → Unique identifier
- Value → Data associated with the key

### Example:
```python
user = {
    "username": "admin",
    "password": "12345"
}
```

Here:
- username → Key
- admin → Value

---

## 17. What is the Difference Between a List and a Tuple?

### Answer:

| List | Tuple |
|--------|--------|
| Mutable | Immutable |
| Uses [] | Uses () |
| Can be modified | Cannot be modified |

### Example:
```python
my_list = [1, 2, 3]
my_tuple = (1, 2, 3)
```

---

## 18. What is the Difference Between == and = ?

### Answer:

| Operator | Purpose |
|-----------|----------|
| = | Assignment |
| == | Comparison |

### Example:
```python
x = 10

if x == 10:
    print("Equal")
```

---

## 19. What is a Return Statement?

### Answer:
The return statement sends a value back from a function.

### Example:
```python
def multiply(a, b):
    return a * b

result = multiply(5, 4)
print(result)
```

### Output:
```
20
```

---

## 20. What is the Difference Between print() and return?

### Answer:

| print() | return |
|----------|---------|
| Displays output | Sends value back |
| Used for viewing | Used for processing |

### Example:
```python
def test():
    print("Hello")

def test2():
    return "Hello"
```

## 21. What are the main features of Python?

### Answer:
- Easy to learn: Python has simple and readable syntax.
- Interpreted: Python code is executed by the Python interpreter.
- Dynamically typed: We don't need to declare the data type of a variable explicitly.
- Object-oriented: Python supports classes, objects, inheritance, polymorphism, etc.
- High-level language: It abstracts many low-level programming details, such as manual memory management.
- Portable: Python programs can run on different operating systems with suitable Python environments.
-Open-source: Python is freely available to use and modify.
- Extensive libraries: Python provides libraries for data analysis, machine learning, web development, automation and more.
- Extensible: Python can work with code written in other languages, such as C and C++.


## 22. Is Python Compiled or Interpreted?

### Answer:
Python is generally considered an interpreted language, but internally it uses both compilation and interpretation.
When we execute a Python program:

1. The Python source code (`.py`) is compiled into bytecode.
2. The Python Virtual Machine (PVM) executes that bytecode.

### Example:
```python
print("Hello World")
```

### Output:
```text
Hello World
```

## 7. What is the Difference Between Compiled and Interpreted Languages?

### Answer:

| Compiled Language | Interpreted Language |
|---|---|
| Source code is compiled before execution. | Source code is executed through an interpreter. |
| Traditionally produces machine code or an executable. | Traditionally executes instructions through an interpreter. |
| Compilation can identify certain errors before execution. | Many errors are encountered during execution. |
| Examples: C and C++. | Examples: Python and JavaScript. |

 The distinction is not absolute. Python also performs compilation internally, and modern JavaScript engines use compilation techniques.


## 23. Is Python a Dynamically Typed Language?

### Answer:
Yes, Python is a dynamically typed language. It means that we don't need to explicitly declare the data type of a variable. Python determines the type at runtime based on the value assigned to it.

### Example:
```python
x = 10
print(type(x))

x = "Hello"
print(type(x))

x = 10.5
print(type(x))
```

### Output:
```text
<class 'int'>
<class 'str'>
<class 'float'>
```

## 24. What Does Dynamically Typed Mean?

### Answer:
Dynamically typed means that the type associated with a variable is determined during program execution rather than being explicitly declared beforehand. In Python, a variable can refer to different types of objects during program execution.

### Example:
```python
a = 100
print(type(a))

a = "Python"
print(type(a))

a = 25.5
print(type(a))
```

### Output:
```text
<class 'int'>
<class 'str'>
<class 'float'>
```

### Difference Between Static and Dynamic Typing:

| Static Typing | Dynamic Typing |
|---|---|
| Variable types are checked before program execution, typically during compilation. | Types are checked at runtime. |
| Variables generally have declared or inferred fixed types. | A variable can refer to objects of different types. |
| Example: C, C++. | Example: Python, JavaScript. |
