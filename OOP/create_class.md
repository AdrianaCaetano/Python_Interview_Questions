## How do you create a class in Python?

To create a class in python, we use the keyword **“class”** using the syntax `class ClassName (parameters):` and define a `__init__` method to create objects.
```
class Employee:
   def __init__(self, emp_name):
       self.emp_name = emp_name
```
To instantiate or create an object from the class created above, we do the following:
```
emp_1 = Employee("John Smith")
```
To access the name attribute, we just call the attribute using the dot operator as shown below:
```
print(emp_1.emp_name)  #Output:  John Smith
```
To create methods inside the class, we include the methods under the scope of the class as shown below:
```
class Employee:
   def __init__(self, emp_name):
       self.emp_name = emp_name
       
   def introduce(self):
       print("Hello I am " + self.emp_name)
```
The self parameter in the init and introduce functions represent the reference to the current class instance which is used for accessing attributes and methods of that class. 
The self parameter has to be the first parameter of any method defined inside the class. 
The method of the class Employee can be accessed as shown below:
```
emp_1.introduce()
```
