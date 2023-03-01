## What is the difference bettween range() and enumerate()?

`range()` is a built-in function used to iterate through a sequence of numbers.
```
list(range(5))

Output: 
[0, 1, 2, 3, 4]
```

`enumerate()` is a built-in function to iterate through a sequence and keep track of both the index and the value. You can pass in an optional start parameter to indicate which number the index should start at.
```
list(enumerate([1, 2, 3], start=10))

Output:
[(10, 1), (11, 2), (12, 3)]
```

Example: Solve the classic interview question known as Fizz Buzz using `enumerate()`
```
# use range() tto create a list of numbers
numbers = [i for i in range(10)]
print(numbers)

Output:
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

# Use enumerate to solve FizzBuzz
for i, num in enumerate(numbers):
    if num % 5 == 0 and num % 3 == 0:
        numbers[i] = "fizzbuzz"
    elif num % 3 == 0:
        numbers[i] = "fizz"
    elif num % 5 == 0:
        numbers[i] = "buzz"
print(numbers)

Output:
['fizzbuzz', 1, 2, 'fizz', 4, 'buzz', 'fizz', 7, 8, 'fizz']
```
