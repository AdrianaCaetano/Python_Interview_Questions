## What are global, protected and private attributes in Python?

**Global** variables are public variables that are defined in the global scope. To use the variable in the global scope inside a function, we use the `global` keyword.

**Protected** attributes are attributes defined with an underscore prefixed to their identifier eg. and `_sara`. They can still be accessed and modified from outside the class they are defined in but a responsible developer should refrain from doing so.

**Private** attributes are attributes with double underscore prefixed to their identifier eg. `__ansh`. They cannot be accessed or modified from the outside directly and will result in an `AttributeError` if such an attempt is made.
