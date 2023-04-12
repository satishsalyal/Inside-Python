
# Nested loops and control statements

In Python, we can use nested loops to iterate over multiple sequences or to perform operations on multidimensional data
structures. Nested loops are simply loops that are placed inside another loop. 
The syntax for a nested loop is as follows:

```python

for outer_loop_var in outer_sequence:
    for inner_loop_var in inner_sequence:
        # code to execute for each combination of outer_loop_var and inner_loop_var
```
In this example, we have an outer loop that iterates over the elements of an outer sequence, and an inner loop
that iterates over the elements of an inner sequence. The code block under the nested loop is executed for each 
combination of outer_loop_var and inner_loop_var.

Here's an example of a nested loop that prints out the multiplication table from 1 to 10:

```python

for i in range(1, 11):
    for j in range(1, 11):
        print(i*j, end="\t")
    print()
```
In this example, we have an outer loop that iterates over the numbers from 1 to 10, and an inner loop that iterates 
over the numbers from 1 to 10. The code block under the nested loop prints out the product of the two numbers, 
separated by a tab, and then prints a newline character to move to the next row.

## break and continue

In Python, the *break and continue* statements are used to control the flow of execution within loops.

The break statement is used to terminate the current loop prematurely, and move on to the next statement 
that follows the loop. This is particularly useful when you want to stop the loop once a certain condition has been met.
Here's an example of using break in a while loop:

```python

i = 1
while i < 10:
    if i == 5:
        break
    print(i)
    i += 1
```
In this example, the loop will run as long as i is less than 10. However, if i ever equals 5, the break 
statement is executed, and the loop is terminated prematurely. So the output of this code will be:
**1
  2
  3
  4**
  
The continue statement is used to skip the current iteration of the loop, and move on to the next iteration. 
This is particularly useful when you want to skip certain iterations based on a certain condition, without actually 
terminating the loop altogether. Here's an example of using continue in a for loop:

```python

for i in range(1, 11):
    if i % 2 == 0:
        continue
    print(i)
```  
 
 In this example, the loop iterates over the numbers from 1 to 10. However, if i is even, the continue statement is 
 executed, and the current iteration of the loop is skipped. So the output of this code will be:


**1
  3
  5
  7
  9**
Both break and continue can also be used within nested loops to control the flow of execution within the inner loop. 
Just remember that break will only exit the innermost loop that it's placed in, while continue will only skip the 
current iteration of the innermost loop that it's placed in.

We can also use control statements like *"break" and "continue"* to control the behavior of nested loops. 
"break" is used to exit the innermost loop immediately, while "continue" is used to skip to the next iteration of 
the innermost loop. Here's an example of using "break" and "continue" in a nested loop:

```python

for i in range(1, 6):
    for j in range(1, 6):
        if i*j > 15:
            break
        elif i*j == 5:
            continue
        else:
            print(i*j, end=" ")
    print()
 ```
In this example, we have an outer loop that iterates over the numbers from 1 to 5, and an inner loop that iterates 
over the numbers from 1 to 5. The code block under the nested loop prints out the product of the two numbers, separated 
by a space, if the product is less than or equal to 15 and is not equal to 5. If the product is greater than 15, 
the inner loop is exited using "break". If the product is equal to 5, the current iteration of the inner loop is 
skipped using "continue".

I hope these examples help you understand how to *use nested loops and control statements* in Python to iterate over 
multiple sequences and perform operations on multidimensional data structures.
