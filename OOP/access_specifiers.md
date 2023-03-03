## Are access specifiers used in python?

Python does not make use of access specifiers specifically like private, public, protected, etc. 
However, it does not derive this from any variables. 
It has the concept of imitating the behaviour of variables by making use of a single (protected) or double underscore (private) as prefixed to the variable names. 
By default, the variables without prefixed underscores are public.

```
# to demonstrate access specifiers
class InterviewbitEmployee:
   
    # protected members
    _emp_name = None
    _age = None
    
    # private members
    __branch = None
    
    # constructor
    def __init__(self, emp_name, age, branch): 
         self._emp_name = emp_name
         self._age = age
         self.__branch = branch
    
    #public member
    def display():
        print(self._emp_name +" "+self._age+" "+self.__branch)
```
