# Classes and Objects

# Resources
1. [Object Oriented Programming](https://python.swaroopch.com/oop.html)(Read everything until the paragraph “Inheritance” excluded. You do NOT have to learn about class attributes, `classmethod` and `staticmethod` yet)
2. [Object-Oriented Programming](https://python-course.eu/oop/object-oriented-programming.php)(Please *be careful*: in most of the following paragraphs, the author shows things the way you should not use or write a class in order to help you better understand some concepts and how everything works in Python 3. Make sure you read everything in the following paragraphs: General Introduction, First-class Everything, A Minimal Class in Python, Attributes (You DON’T have to learn about class attributes), Methods, The `__init__` Method, “Data Abstraction, Data Encapsulation, and Information Hiding,” “Public, Protected, and Private Attributes”)
3. [Properties vs. Getters and Setters](https://python-course.eu/oop/properties-vs-getters-and-setters.php)
4. [Learn to Program 9 : Object Oriented Programming](https://www.youtube.com/watch?v=1AGyBuVCTeE)
5. [Python Classes and Objects](https://www.youtube.com/watch?v=apACNr7DC_s)
6. [Object Oriented Programming](https://www.youtube.com/watch?v=-DP1i2ZU9gk)

# Learning Objectives
At the end of this project, you are expected to be able to [explain to anyone](https://fs.blog/feynman-learning-technique/?fbclid=IwAR2K5_BGPVo0QjJXkOIIqNsqcXK4lTskPWJvA0asKQIGtCPWaQBdKmj1Ztg), **without the help of Google:**

## General
* Why Python programming is awesome
* What is OOP
* “first-class everything”
* What is a class
* What is an object and an instance
* What is the difference between a class and an object or instance
* What is an attribute
* What are and how to use public, protected and private attributes
* What is `self`
* What is a method
* What is the special `__init__` method and how to use it
* What is Data Abstraction, Data Encapsulation, and Information Hiding
* What is a property
* What is the difference between an attribute and a property in Python
* What is the Pythonic way to write getters and setters in Python
* How to dynamically create arbitrary new attributes for existing instances of a class
* How to bind attributes to object and classes
* What is the `__dict__` of a class and/or instance of a class and what does it contain
* How does Python find the attributes of an object or class
* How to use the `getattr` function

# Requirements
## General
* Allowed editors: `vi`, `vim`, `emacs`
* All your files will be interpreted/compiled on Ubuntu 20.04 LTS using python3 (version 3.8.5)
* All your files should end with a new line
* The first line of all your files should be exactly `#!/usr/bin/python3`
* A `README.md` file, at the root of the folder of the project, is mandatory
* Your code should use the pycodestyle (version `2.8.*`)
* All your files must be executable
* The length of your files will be tested using `wc`
* All your modules should have a documentation (`python3 -c 'print(__import__("my_module").__doc__)'`)
* All your classes should have a documentation (`python3 -c 'print(__import__("my_module").MyClass.__doc__)'`)
* All your functions (inside and outside a class) should have a documentation 
(`python3 -c 'print(__import__("my_module").my_function.__doc__)'` and `python3 -c 'print(__import__("my_module").MyClass.my_function.__doc__)'`)
* A documentation is not a simple word, it’s a real sentence explaining what’s the purpose of the module, class or method (the length of it will be verified)

# More Info
**Documentation is now mandatory!** Each module, class, and method must contain docstring as comments. [Example Google Style Python Docstrings](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html)

# Tasks
Tasks table

| Task Name  | File Name | Description |
| --------------- | ------------------------------ |---------------------------------------------------------------|
| 0. My first square | `0-square.py`  | An empty class `Square` that defines a square |
| 1. Square with size | `1-square.py` | A class `Square` that defines a square |
| 2. Size validation | `2-square.py` | A class `Square` that defines a square by: (based on `1-square.py`) |
| 3. Area of a square | `3-square.py` | A class `Square` that defines a square by: (based on `2-square.py`) |
| 4. Access and update private attribute | `4-square.py` | A class `Square` that defines a square by: (based on `3-square.py`) |
| 5. Printing a square | `5-square.py` | A class `Square` that defines a square by: (based on `4-square.py`) |
| 6. Coordinates of a square | `6-square.py` | A class `Square` that defines a square by: (based on `5-square.py`) |
| 7. Singly linked list | `100-singly_linked_list.py` | A class `Node` that defines a node of a singly linked list |
| 8. Print Square instance | `101-square.py` | A class `Square` that defines a square by: (based on `6-square.py`) |
| 9. Compare 2 squares | `102-square.py` | A class `Square` that defines a square by: (based on `4-square.py`) |
| 10. ByteCode -> Python #5 | `103-magic_class.py` | A Python class `MagicClass` |
