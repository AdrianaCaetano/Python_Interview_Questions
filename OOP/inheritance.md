## How does inheritance work in python? Explain it with an example.

Inheritance gives the power to a class to access all attributes and methods of another class. 
It aids in code reusability and helps the developer to maintain applications without redundant code. 
The class inheriting from another class is called child class or derived class. 
The class from which a child class derives the members are called parent class or superclass.

Python supports different kinds of inheritance, they are:

### Single Inheritance

Child class derives members of one parent class.

```
# Parent class
class ParentClass:
    def par_func(self):
         print("I am parent class function")

# Child class
class ChildClass(ParentClass):
    def child_func(self):
         print("I am child class function")

# Driver code
obj1 = ChildClass()
obj1.par_func()
obj1.child_func()
```

### Multi-level Inheritance

The members of the parent class, A, are inherited by child class which is then inherited by another child class, B. 
The features of the base class and the derived class are further inherited into the new derived class, C. 
Here, A is the grandfather class of class C.

```
# Parent class
class A:
   def __init__(self, a_name):
       self.a_name = a_name
   
# Intermediate class
class B(A):
   def __init__(self, b_name, a_name):
       self.b_name = b_name
       # invoke constructor of class A
       A.__init__(self, a_name)

# Child class
class C(B):
   def __init__(self,c_name, b_name, a_name):
       self.c_name = c_name
       # invoke constructor of class B
       B.__init__(self, b_name, a_name)
       
   def display_names(self):
       print("A name : ", self.a_name)
       print("B name : ", self.b_name)
       print("C name : ", self.c_name)

#  Driver code
obj1 = C('child', 'intermediate', 'parent')
print(obj1.a_name)
obj1.display_names()
```

### Multiple Inheritance
This is achieved when one child class derives members from more than one parent class. 
All features of parent classes are inherited in the child class.

```
# Parent class1
class Parent1:
   def parent1_func(self):
       print("Hi I am first Parent")

# Parent class2
class Parent2:
   def parent2_func(self):
       print("Hi I am second Parent")

# Child class
class Child(Parent1, Parent2):
   def child_func(self):
       self.parent1_func()
       self.parent2_func()

# Driver's code
obj1 = Child()
obj1.child_func()
```

### Hierarchical Inheritance

When a parent class is derived by more than one child class, it is called hierarchical inheritance.

```
# Base class
class A:
     def a_func(self):
         print("I am from the parent class.")

# 1st Derived class
class B(A):
     def b_func(self):
         print("I am from the first child.")

# 2nd Derived class
class C(A):
     def c_func(self):
         print("I am from the second child.")
 
# Driver's code
obj1 = B()
obj2 = C()
obj1.a_func()
obj1.b_func()    #child 1 method
obj2.a_func()
obj2.c_func()    #child 2 method
```


