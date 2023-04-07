## Understanding variables, data types and data structures in Python

Python is a versatile and powerful programming language that is widely used in the industry. One of the essential concepts of Python is understanding variables, data types, and data structures. In this chapter, we will explore these concepts in detail, along with examples.

### Variables

Variables are used to store data in a program. They act as containers that hold values, such as numbers, strings, or other data types. In Python, variables are dynamically typed, which means that their data type can change at runtime. To create a variable in Python, you need to assign a value to it using the assignment operator (=).

For example:

```python
x = 10
y = "hello"
```
In this example, we have created two variables, x and y, and assigned them the values 10 and "hello," respectively. Note that we did not need to declare the data type explicitly.

#### Data Types

Python has several built-in data types, including numbers, strings, lists, tuples, sets, and dictionaries. Each data type has specific properties and functions. Understanding data types is essential in Python because it helps you manipulate data effectively.

## Let's explore each data type in detail.

### Numbers

Python supports various numerical data types, such as integers, floating-point numbers, and complex numbers. You can perform arithmetic operations on numbers, such as addition, subtraction, multiplication, and division.

For example:

```python
a = 5
b = 2.5
c = a + b
print(c)
```
In this example, we have created two variables, a and b, and assigned them the values 5 and 2.5, respectively. We then added them and assigned the result to the variable c. Finally, we printed the value of c, which is 7.5.

#### Strings

Strings are used to represent textual data in Python. They are enclosed in quotes, either single ('') or double (""). In Python, strings are immutable, which means that you cannot change the value of a string after it is created.

For example:

```pyhton
name = "John"
print("My name is", name)
```
In this example, we have created a variable called name and assigned it the value "John." We then printed a message that includes the variable name.

### Lists

A list is an ordered collection of items. It can contain elements of different data types and is mutable, which means that you can add, remove, or modify elements in a list.

For example:

```python
fruits = ["apple", "banana", "orange"]
fruits.append("grape")
print(fruits)
```
In this example, we have created a list called fruits and initialized it with three elements: "apple," "banana," and "orange." We then added a fourth element, "grape," using the append method. Finally, we printed the contents of the fruits list.

### Tuples

Tuples are similar to lists, but they are immutable. Once created, you cannot modify their values. Tuples are often used to group related data together, and they are more memory-efficient than lists.

For example:

```python
person = ("John", 25, "male")
print(person)
```
In this example, we have created a tuple called person and assigned it the values "John," 25, and "male." We then printed the contents of the person tuple.

### Sets

Sets are unordered collections of unique elements. They are mutable, which means that you can add or remove elements



