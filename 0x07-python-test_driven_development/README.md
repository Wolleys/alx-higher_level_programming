# Test-driven development

# Resources
1. [doctest — Test interactive Python examples (until “26.2.3.7. Warnings” included)](https://docs.python.org/3.4/library/doctest.html)
2. [doctest – Testing through documentation](https://pymotw.com/3/doctest/)
3. [Unit Tests in Python](https://www.youtube.com/watch?v=1Lfv5tUGsn8)
4. [Unittest module](https://www.youtube.com/watch?v=6tNS--WetLI)
5. [Interactive and Non-interactive tests](https://mattermost.com/blog/testing-python-understanding-doctest-and-unittest/)

# Learning Objectives
At the end of this project, you are expected to be able to [explain to anyone](https://fs.blog/feynman-learning-technique/?fbclid=IwAR2K5_BGPVo0QjJXkOIIqNsqcXK4lTskPWJvA0asKQIGtCPWaQBdKmj1Ztg),
**without the help of Google:**

## General
* Why Python programming is awesome
* What’s an interactive test
* Why tests are important
* How to write Docstrings to create tests
* How to write documentation for each module and function
* What are the basic option flags to create tests
* How to find edge cases

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
* A documentation is not a simple word, it’s a real sentence explaining what’s the purpose of the module, class or method (the length of it will be verified)

# Tasks
Tasks table

| Task Name  | File Name | Description |
| --------------- | ------------------------------ |---------------------------------------------------------------|
| 0. Integers addition | `0-add_integer.py, tests/0-add_integer.txt` | Add 2 integers |
| 1. Divide a matrix | `2-matrix_divided.py, tests/2-matrix_divided.txt` | Divide all elements of a matrix |
| 2. Say my name | `3-say_my_name.py, tests/3-say_my_name.txt` | Print `My name is <first name> <last name>` |
| 3. Print square | `4-print_square.py, tests/4-print_square.txt` | Print a square with the character `#` |
| 4. Text indentation | `5-text_indentation.py, tests/5-text_indentation.txt` | Print a text with 2 new lines after each of these characters: `.`, `?` and `:` |
| 5. Max integer - Unittest | `tests/6-max_integer_test.py` | unittests for the function `def max_integer(list=[]):` |
| 6. Matrix multiplication | `100-matrix_mul.py, tests/100-matrix_mul.txt` | Multiply 2 matrices |
| 7. Lazy matrix multiplication | `101-lazy_matrix_mul.py, tests/101-lazy_matrix_mul.txt` | Multiply 2 matrices by using the module [NumPy](https://numpy.org) |
| 8. CPython #3: Python Strings | `102-python.c` | Print Python strings |















