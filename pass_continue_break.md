## What is the difference between pass, continue and break in python?

In Python, **pass**, **continue**, and **break** are three different keywords that are used for controlling the flow of execution in loops or conditional statements.

### pass 
It is a null operation, which means that it doesn't do anything. The pass keyword in Python is generally used to fill up empty blocks and is similar to an empty statement represented by a semi-colon in languages such as Java, C++, Javascript, etc.

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
It is used to skip the current iteration of a loop and move on to the next iteration. It is used when you want to skip some part of the loop for a specific condition. The continue statement terminates the current iteration of the statement, skips the rest of the code in the current iteration and the control flows to the next iteration of the loop.
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
The break statement terminates the loop immediately and the control flows to the statement after the body of the loop. It is used when you want to exit the loop or conditional statement prematurely. 
```
Example:
for i in range(10):
  if i == 5:
    break
  else:
    print(I)
```
In this example, the break keyword is used to exit the loop when i is equal to 5, so the program will move on to the next statement in the program.


Example of using pass, break, and continue in a loop:
```
pat = [1, 3, 2, 1, 2, 3, 1, 0, 1, 3]
for p in pat:
   pass  # do nothing
   if (p == 0):
       current = p
       break # exit the loop
   elif (p % 2 == 0):
       continue # move to the next iteration
   print(p)    # output => 1 3 1 3 1
   
print(current)    # output => 0
```
