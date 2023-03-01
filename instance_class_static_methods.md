## What is the difference between Instance Method, Class Method, and Static Method?

### Instance Method
Instance methods are the most commonly used type of method in Python. They are associated with an instance of a class, which means that they can access and modify the state of the instance. They are defined with the self parameter in the method definition. This parameter refers to the instance of the class that the method is being called on.

Example of instance method:
```
class MyClass:
  def __init__(self, value):
    self.value = value

  def double_value(self):
    return self.value * 2

my_instance = MyClass(10)
print(my_instance.double_value()) # Output: 20
```

### Class Method
Class methods are similar to instance methods, but they are associated with the class rather than an instance of the class. They are defined with the @classmethod decorator and have access to the class and class state through the cls parameter.

Example of class method:
```
class MyClass:
  count = 0

  def __init__(self):
    MyClass.count += 1

  @classmethod
  def get_count(cls):
    return cls.count

my_instance1 = MyClass()
my_instance2 = MyClass()
print(MyClass.get_count()) # Output: 2
```

### Static Method
Static methods are methods that are not associated with an instance of a class. They are defined with the @staticmethod decorator and do not have access to the instance or class state. They are commonly used for utility functions that do not require any instance or class state to operate.

Example of staticmethod:
```
class MyClass:
  @staticmethod
  def say_hello():
    print("Hello!")

MyClass.say_hello() # Output: "Hello!"
```

### Summary
The main difference between instance, static, and class methods in Python is that instance methods are associated with an instance of a class, static methods are not associated with an instance or class, and class methods are associated with the class itself.




#### Reference: 
*[Sashi Sharma](https://www.linkedin.com/in/sakshi-sharma-a80985229/) post on LinkedIn*
