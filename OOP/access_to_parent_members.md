## How do you access parent members in the child class?

Following are the ways using which you can access parent class members within a child class:

### By using Parent class name

You can use the name of the parent class to access the attributes as shown in the example below:
```
class Parent(object):  
   # Constructor
   def __init__(self, name):
       self.name = name    
 
class Child(Parent): 
   # Constructor
   def __init__(self, name, age):
       Parent.name = name
       self.age = age
 
   def display(self):
       print(Parent.name, self.age)
 
# Driver Code
obj = Child("Anna", 6)
obj.display()
```

### By using super()

The parent class members can be accessed in child class using the `super` keyword.
```
class Parent(object):
   # Constructor
   def __init__(self, name):
       self.name = name    
 
class Child(Parent):
   # Constructor
   def __init__(self, name, age):         
       ''' 
       In Python 3.x, we can also use super().__init__(name)
       ''' 
       super(Child, self).__init__(name)
       self.age = age
 
   def display(self):
      # Note that Parent.name cant be used 
      # here since super() is used in the constructor
      print(self.name, self.age)
  
# Driver Code
obj = Child("Anna", 6)
obj.display()
```
