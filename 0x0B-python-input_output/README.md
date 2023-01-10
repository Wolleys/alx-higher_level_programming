# Input/Output

# Resources
1. [7.2. Reading and Writing Files](https://docs.python.org/3/tutorial/inputoutput.html#reading-and-writing-files)
2. [8.7. Predefined Clean-up Actions](https://docs.python.org/3/tutorial/errors.html#predefined-clean-up-actions)
3. [Dive Into Python 3: Chapter 11. Files](https://histo.ucsf.edu/BMS270/diveintopython3-r802.pdf) (*until “11.4 Binary Files” (included)*)
4. [JSON encoder and decoder](https://docs.python.org/3/library/json.html)
5. [Learn to Program 8 : Reading / Writing Files](https://www.youtube.com/watch?v=EukxMIsNeqU)
6. [Automate the Boring Stuff with Python](https://automatetheboringstuff.com) (*ch. 8 p 180-183 and ch. 14 p 326-333*)
7. [All about py-file I/O](https://techvidvan.com/tutorials/python-file-read-write/)

# Learning Objectives
At the end of this project, you are expected to be able to [explain to anyone](https://fs.blog/feynman-learning-technique/?fbclid=IwAR2K5_BGPVo0QjJXkOIIqNsqcXK4lTskPWJvA0asKQIGtCPWaQBdKmj1Ztg), **without the help of Google:**

# General
* Why Python programming is awesome
* How to open a file
* How to write text in a file
* How to read the full content of a file
* How to read a file line by line
* How to move the cursor in a file
* How to make sure a file is closed after using it
* What is and how to use the `with` statement
* What is `JSON`
* What is serialization
* What is deserialization
* How to convert a Python data structure to a JSON string
* How to convert a JSON string to a Python data structure

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

# Tasks
Tasks table

| Task Name  | File Name | Description |
| --------------- | ------------------------------ |---------------------------------------------------------------|
| 0. Read file | `0-read_file.py` | Read a text file (`UTF8`) and prints it to stdout |
| 1. Write to a file | `1-write_file.py` | Write a string to a text file (`UTF8`) |
| 2. Append to a file | `2-append_write.py` | Append a string at the end of a text file (`UTF8`) |
| 3. To JSON string | `3-to_json_string.py` | Return the JSON representation of an object (string) |
| 4. From JSON string to Object | `4-from_json_string.py` | Return an object (Python data structure) represented by a JSON string |
| 5. Save Object to a file | `5-save_to_json_file.py` | Write an Object to a text file, using a JSON representation |
| 6. Create object from a JSON file | `6-load_from_json_file.py` | Create an Object from a `“JSON file”` |
| 7. Load, add, save | `7-add_item.py` | Add all arguments to a Python list, and then save them to a file |
| 8. Class to JSON | `8-class_to_json.py` | Return the dictionary description with simple data structure |
| 9. Student to JSON | `9-student.py` | A class `Student` that defines a student by |
| 10. Student to JSON with filter | `10-student.py` | A class `Student` that defines a student by: (based on `9-student.py`) |
| 11. Student to disk and reload | `11-student.py` | A class `Student` that defines a student by: (based on `10-student.py`) |
| 12. Pascal's Triangle | `12-pascal_triangle.py` | A function `def pascal_triangle(n)` |
| 13. Search and update | `100-append_after.py` | Insert a line of text to a file, |
| 14. Log parsing | `101-stats.py` | Read the `stdin` line by line and computes metrics |
