## What is the difference between pass, continue and break in python?

In Python, **pass**, **continue**, and **break** are three different keywords that are used for controlling the flow of execution in loops or conditional statements.

### pass 
It is a null operation, which means that it doesn't do anything. It is used when you need a statement syntactically but you don't want any command or code to execute. For example, if you have an if statement in your code, but you haven't decided what should be done if the condition is true, you can use pass to avoid a syntax error.

```
Example:
for i in range(10):
  if i % 2 == 0:
    pass
  else:
    print(i)
```

In this example, the pass keyword is used to do nothing when i is an even number, so the program will move on to the next iteration of the loop.

### continue
It is used to skip the current iteration of a loop and move on to the next iteration. It is used when you want to skip some part of the loop for a specific condition.
```
Example:
for i in range(10):
  if i % 2 == 0:
    continue
  else:
    print(i)
```
In this example, the continue keyword is used to skip the current iteration of the loop when i is an even number, so the program will move on to the next iteration.

### break 
It is used to terminate the loop or conditional statement and move on to the next statement in the program. It is used when you want to exit the loop or conditional statement prematurely.
```
Example:
for i in range(10):
  if i == 5:
    break
  else:
    print(I)
```
In this example, the break keyword is used to exit the loop when i is equal to 5, so the program will move on to the next statement in the program.
