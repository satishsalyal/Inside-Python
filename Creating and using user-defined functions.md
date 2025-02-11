# Python Functions: Creating, Scoping, and Lambda Expressions

## Introduction
Functions in Python allow developers to write reusable and modular code. Python provides built-in functions, but user-defined functions help organize logic efficiently. This guide covers creating user-defined functions, understanding variable scoping, and using lambda functions effectively.

---

## Creating User-Defined Functions
Python allows you to define your own functions using the `def` keyword. Functions help break down complex code into manageable parts.

### **Syntax:**
```python
def function_name(parameters):
    """Function Docstring (optional)"""
    # Function body
    return result
```

### **Example:**
```python
def greet(name):
    return f"Hello, {name}!"

print(greet("Alice"))  # Output: Hello, Alice!
```

---

## Understanding Scoping and Global Variables
Python follows the **LEGB rule** for variable scope:
- **L**ocal: Defined inside a function.
- **E**nclosing: Defined in outer functions.
- **G**lobal: Defined at the top level of a script/module.
- **B**uilt-in: Predefined names in Python.

### **Example:**
```python
count = 0  # Global variable

def increment():
    global count  # Access and modify the global variable
    count += 1

increment()
print(count)  # Output: 1
```
⚠️ **Note:** Overuse of global variables can make debugging difficult. It's recommended to pass variables explicitly when possible.

---

## Understanding Lambda Functions
Lambda functions are anonymous, one-line functions that can be used where simple, short-lived functions are needed.

### **Syntax:**
```python
lambda arguments: expression
```

### **Example:**
```python
square = lambda x: x * x
print(square(5))  # Output: 25
```

Lambda functions are particularly useful for operations like mapping and sorting:
```python
numbers = [1, 2, 3, 4]
squared_numbers = list(map(lambda x: x**2, numbers))
print(squared_numbers)  # Output: [1, 4, 9, 16]
```

⚡ **Tip:** While lambda functions make code concise, avoid making them overly complex, as it can reduce readability.

---

## Conclusion
Understanding user-defined functions, scope management, and lambda functions allows Python developers to write clean, efficient, and well-structured code. By leveraging functions effectively, you can improve code readability and reusability.

✅ **Next Steps:** Practice by writing your own functions, experimenting with scopes, and using lambda expressions in real-world problems!
