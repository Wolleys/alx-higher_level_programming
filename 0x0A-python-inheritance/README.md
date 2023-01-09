# Inheritance

# Resources
1. [Inheritance](https://docs.python.org/3/tutorial/classes.html#inheritance)
2. [Multiple inheritance](https://docs.python.org/3/tutorial/classes.html#multiple-inheritance)
3. [Inheritance in Python](https://www.geeksforgeeks.org/inheritance-in-python/)
4. [Learn to Program 10 : Inheritance Magic Methods](https://www.youtube.com/watch?v=d8kCdLCi6Lk)

# Learning Objectives
At the end of this project, you are expected to be able to [explain to anyone](https://fs.blog/feynman-learning-technique/?fbclid=IwAR2K5_BGPVo0QjJXkOIIqNsqcXK4lTskPWJvA0asKQIGtCPWaQBdKmj1Ztg), **without the help of Google:**

## General
* Why Python programming is awesome
* What is a superclass, baseclass or parentclass
* What is a subclass
* How to list all attributes and methods of a class or instance
* When can an instance have new attributes
* How to inherit class from another
* How to define a class with multiple base classes
* What is the default class every class inherit from
* How to override a method or attribute inherited from the base class
* Which attributes or methods are available by heritage to subclasses
* What is the purpose of inheritance
* What are, when and how to use `isinstance`, `issubclass`, `type` and `super` built-in functions

# Requirements
## Python Scripts
* Allowed editors: `vi`, `vim`, `emacs`
* All your files will be interpreted/compiled on Ubuntu 20.04 LTS using python3 (version 3.8.5)
* All your files should end with a new line
* The first line of all your files should be exactly `#!/usr/bin/python3`
* A `README.md` file, at the root of the folder of the project, is mandatory
* Your code should use the pycodestyle (version `2.8.*`)
* All your files must be executable
* The length of your files will be tested using `wc`

## Python Test Cases
* Allowed editors: `vi`, `vim`, `emacs`
* All your files should end with a new line
* All your test files should be inside a folder `tests`
* All your test files should be text files (extension: `.txt`)
* All your tests should be executed by using this command: `python3 -m doctest ./tests/*`
* All your modules should have a documentation (`python3 -c 'print(__import__("my_module").__doc__)'`)
* All your classes should have a documentation (`python3 -c 'print(__import__("my_module").MyClass.__doc__)'`)
* All your functions (inside and outside a class) should have a documentation (`python3 -c 'print(__import__("my_module").my_function.__doc__)`' 
and `python3 -c 'print(__import__("my_module").MyClass.my_function.__doc__)'`)

## Documentation
* Do not use the works `import` or `from` inside your comments, the checker will think you try to import some modules

# Tasks
Tasks table

| Task Name  | File Name | Description |
| --------------- | ------------------------------ |---------------------------------------------------------------|
| 0. Lookup | `0-lookup.py` | Return the list of available attributes and methods of an object |
| 1. My list | `1-my_list.py, tests/1-my_list.txt` | A class `MyList` that inherits from `list` |
| 2. Exact same object | `2-is_same_class.py` | Return `True` if the object is exactly an instance of the specified class |
| 3. Same class or inherit from | `3-is_kind_of_class.py` | Return `True` if the object is an instance |
| 4. Only sub class of | `4-inherits_from.py` | Return `True` if the object is an instance of a class that inherited |
| 5. Geometry module | `5-base_geometry.py` | An empty class `BaseGeometry` |
| 6. Improve Geometry | `6-base_geometry.py` | A class `BaseGeometry` (based on `5-base_geometry.py`) |
| 7. Integer validator | `7-base_geometry.py, tests/7-base_geometry.txt` | A class `BaseGeometry` (based on `6-base_geometry.py`) |
| 8. Rectangle | `8-rectangle.py` | A class `Rectangle` that inherits from `BaseGeometry` (`7-base_geometry.py`) |
| 9. Full rectangle | `9-rectangle.py` | A class `Rectangle` that inherits from `BaseGeometry` (`7-base_geometry.py`) |
| 10. Square #1 | `10-square.py` | A class `Square` that inherits from `Rectangle` (`9-rectangle.py`) |
| 11. Square #2 | `11-square.py` | A class `Square` that inherits from `Rectangle` (`9-rectangle.py`) |
| 12. My integer | `100-my_int.py` | A class `MyInt` that inherits from `int` |
| 13. Can I? | `101-add_attribute.py` | Add a new attribute to an object if it’s possible |
