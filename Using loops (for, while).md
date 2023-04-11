# Using loops (for, while)

Loops are a fundamental part of programming, and in Python, we have two types of loops: "for" and "while" loops. 
In this explanation, we'll discuss both types of loops in detail and provide examples for each.

 ## While Loops
 In Python, the "while" loop is used to execute a block of code repeatedly as long as a certain condition is true. There is no "do-while" loop in Python, 
 but we can achieve the same functionality using a "while" loop with a "break" statement. Let's look at each type of loop in detail and provide examples for each.


The syntax for a "while" loop in Python is as follows:

```python

while condition:
    # code to execute as long as the condition is true
```
In this loop, the "condition" is checked before each iteration of the loop. If the condition is true, the code block under the loop is executed, and 
then the condition is checked again. This process repeats until the condition becomes false.

Here's an example of a "while" loop that prints out the numbers from 1 to 5:

```python

i = 1
while i <= 5:
    print(i)
    i += 1
```
In this example, we initialize the variable "i" to 1 and then use a "while" loop to print out the value of "i" and increment it by 1 on each iteration. 
The loop continues until "i" is greater than 5.

We can also use "while" loops to repeatedly ask the user for input until they provide valid input. For example, here's a "while" loop that prompts the user 
for a number and keeps asking until they enter a valid integer:

```python

while True:
    try:
        num = int(input("Enter a number: "))
        break
    except ValueError:
        print("Invalid input. Please enter a valid integer.")
```
In this example, we use a "while" loop with a "try-except" block to repeatedly prompt the user for input and handle any errors that occur. 
The loop continues until the user enters a valid integer, at which point the loop breaks and the program continues executing.

## Do-While Loops
A "do-while" loop is used to execute a block of code at least once, and then repeatedly execute the block as long as a certain condition is true. 
In Python, there is no built-in "do-while" loop, but we can achieve the same functionality using a "while" loop with a "break" statement. Here's an example:

```python

while True:
    # code to execute at least once
    num = int(input("Enter a number: "))
    if num == 0:
        break
```
In this example, we use a "while" loop with a "break" statement to repeatedly ask the user for a number until they enter 0.
The loop executes at least once, since the code block is executed before the condition is checked. Then, on each iteration, the user is prompted for a number, 
and if they enter 0, the loop breaks and the program continues executing.


## For Loop

In Python, the "for" loop is used to iterate over a sequence of elements, such as a list or a string. The syntax for a "for" loop in Python is as follows:

```python

for element in sequence:
    # code to execute for each element
```
In this loop, "sequence" is the sequence of elements to iterate over, and "element" is a variable that takes on each element of the sequence in turn. 
The code block under the loop is executed for each element of the sequence in turn.

Here's an example of a "for" loop that prints out the elements of a list:

```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
```
In this example, we have a list of fruits, and we use a "for" loop to iterate over the elements of the list and print them out one by one.
The loop ends when all the elements of the list have been processed.

We can also use "for" loops to iterate over a range of numbers. For example, here's a "for" loop that prints out the numbers from 1 to 5:

```python

for i in range(1, 6):
    print(i)
```
In this example, we use the built-in "range" function to generate a sequence of numbers from 1 to 5, and then use a "for" loop to iterate over the sequence 
and print out each number in turn.

We can also use "for" loops to iterate over the characters of a string. For example, here's a "for" loop that prints out the characters of a string:

```python

word = "hello"
for char in word:
    print(char)
```
In this example, we use a "for" loop to iterate over the characters of the string "hello" and print them out one by one.

Finally, we can use "for" loops to iterate over the key-value pairs of a dictionary. For example, here's a "for" loop that prints out the keys and values 
of a dictionary:

```python
Copy code
my_dict = {"apple": 1, "banana": 2, "cherry": 3}
for key, value in my_dict.items():
    print(key, value)
```
In this example, we use a "for" loop to iterate over the key-value pairs of the dictionary "my_dict" and print out each key-value pair one by one.
