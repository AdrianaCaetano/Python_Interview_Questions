## What are dictionary and list comprehensions and how we can use them in Python?

Dictionary and list comprehensions are just another concise way to define dictionaries and lists. 

#### List comprehension example:
```
# syntax: [<expr> for <elem> in <lst> if <cond>]
x = [i for i in range(1,5)]
print(x)

Output:
[1, 2, 3, 4]
````
It is the same as:
```
x = list()

for i in range(1,5):
    x.append(i)

print(x)

Output:
[1, 2, 3, 4]
```

List comprehension is used in place of functions like `map()` and `filter()`.

#### Dictionary comprehension example:
```
x = {f"key{i}": i for i in range(5)}
print(x)

Output:
{'key0': 0, 'key1': 1, 'key2': 2, 'key3': 3, 'key4': 4}
```
It is the same as:
```
x = dict()

for i in range(5):
    x[f"key{i}"] = i

print(x)

Output:
{'key0': 0, 'key1': 1, 'key2': 2, 'key3': 3, 'key4': 4}
```
