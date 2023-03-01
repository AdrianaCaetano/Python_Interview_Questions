## What is the difference between Append and Extend in Python?

In Python, the `append()` and `extend()` methods are used to add elements to a list, but they behave differently.

### append()
The `append()` method is used to **add a single element** to the end of a list. For example:
```
a = [1, 2, 3]
a.append(4)
print(a)

Output:
[1, 2, 3, 4]
```

### extend()
The `extend()` method is used to **add multiple elements** to a list. It takes an iterable object (such as a list, tuple, or set) as an argument and adds each element of that iterable to the end of the list. For example:
```
a = [1, 2, 3]
a.extend([4, 5, 6])
print(a)

Output:
[1, 2, 3, 4, 5, 6]
```
So, in summary, the `append()` method is used to add a single element to the end of a list, while the `extend()` method is used to add multiple elements to the end of a list.
