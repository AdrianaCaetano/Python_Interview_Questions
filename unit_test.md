## What are unit tests in Python?

Unit tests are segments of code written to test other pieces of code, typically a single function or method, that we refer to as a unit. 
They are a very important part of the software development process, as they help to ensure that code works as intended and catch bugs early on. 
Also, testing is a best practice that can save time and money by finding and fixing issues before they cause major problems.

The **unittest** module is a framework of Python. The module works based on some important object-oriented concepts. 
A test case is considered a single unit of testing, and it’s represented by the TestCase class. 
Among the numerous tools provided by unittest that allow us to test code, this class is one of the most important ones. 
It’s important to say that all assert methods in the TestCase class also take a msg argument that is used as an error message in case the test fails.

The **unittest** is used as a base class to create our own test cases that enable us to run multiple tests at once.
Unit testing means testing different components of software separately. 
It is necessary to test each and every component properly so that we know which component might be responsible for the failure of the software.

Examples of unit tests on this [DataQuest](https://www.dataquest.io/blog/unit-tests-python/) post.
