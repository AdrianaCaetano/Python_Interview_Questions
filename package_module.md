## Differentiate between a package and a module in python

The **module** is a single python file. A module can import other modules (other python files) as objects. Whereas, a **package** is the folder/directory where different sub-packages and the modules reside.

A python module is created by saving a file with the extension of `.py`. This file will have classes and functions that are reusable in the code as well as across modules.

A python package is created by following the below steps:

- Create a directory and give a valid name that represents its operation.
- Place modules of one kind in this directory.
- Create `__init__.py` file in this directory. This lets python know the directory we created is a package. The contents of this package can be imported across different modules in other packages to reuse the functionality.
