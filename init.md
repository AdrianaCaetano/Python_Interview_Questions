## What is __ init __?

`__init__` is a contructor method in Python and is automatically called to allocate memory when a new object/instance is created. 
All classes have a `__init__` method associated with them. 
It helps in distinguishing methods and attributes of a class from local variables.

```
# class definition
class Student:
   def __init__(self, fname, lname, age, section):
       self.firstname = fname
       self.lastname = lname
       self.age = age
       self.section = section

# creating a new object
stu1 = Student("Anna", "Smith", 22, "A2")
``
