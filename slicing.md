## What is slicing in Python?

As the name suggests, ‘slicing’ is taking parts of.
The syntax for slicing is `[start : stop : step]`
  - **start** is the starting index or where to begin    
  - **stop** is the ending index or where to end    
  - **step** is the size of the step, or how many element to jump
    
The default values for start is 0, for stop is the total number of items, and for step is 1.

Slicing can be done on strings, arrays, lists, and tuples.

```
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
print(numbers[1 : : 2])  #output : [2, 4, 6, 8, 10]
```
