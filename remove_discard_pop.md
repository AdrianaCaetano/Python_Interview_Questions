## Difference between `remove()`, `discard()`, and `pop()` in Python Set.

The set data structure in Python stores unique values, unordered.
```
my_set = {1,2,3,1,2,2,3,3,3,4,4,4}
print(my_set)

Output:
{1, 2, 3, 4}
```

- `remove()` method: 
This method is used to remove an item from a given set in Python. We pass the item name as an argument to the method. But if the passed argument doesn't exist in the set, it will throw an error.
```
# Remove an existing element
my_set.remove(1)
print(my_set)

Output:
{2, 3, 4}

# Remove an unexisting element
my_set.remove(0) 
print(my_set)

Output:
KeyError                                  Traceback (most recent call last)
<ipython-input-5-2f43804aece7> in <module>
----> 1 my_set.remove(0)
      2 print(my_set)

KeyError: 0
```

- `discard()` method: 
Like remove() method, discard() is also used to delete an item from a Python set. But unlike the remove() method, it doesn't throw an error if the item to be deleted doesn't exist.
```
# Discard an existing element
my_set.discard(3)
print(my_set)

Output:
{2, 4}

# Discard an unexisting element
my_set.discard(0)
print(my_set)

Output:
{2, 4}
```

- `pop()` method: 
Like lists in Python, pop() method can also be used to delete an item. The pop() function deletes the last element of the collection. But as sets are unordered , it is hard to predict which item gets deleted. So, better not to use it. The return type of the pop() method is the element popped.
```
my_set.pop()

Output:
2
```
