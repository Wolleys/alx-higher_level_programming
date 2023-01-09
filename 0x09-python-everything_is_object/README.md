# Everything is object

# Resources
1. [9.10. Objects and values](http://www.openbookproject.net/thinkcs/python/english2e/ch09.html#objects-and-values)
2. [9.11. Aliasing](http://www.openbookproject.net/thinkcs/python/english2e/ch09.html#aliasing)
3. [Immutable vs mutable types](https://stackoverflow.com/questions/8056130/immutable-vs-mutable-types)
4. [Mutation](http://composingprograms.com/pages/24-mutable-data.html#sequence-objects) (*Only this chapter*)
5. [9.12. Cloning lists](http://www.openbookproject.net/thinkcs/python/english2e/ch09.html#cloning-lists)
6. [Python tuples: immutable but potentially changing](http://radar.oreilly.com/2014/10/python-tuples-immutable-but-potentially-changing.html)

# Learning Objectives
At the end of this project, you are expected to be able to [explain to anyone](https://fs.blog/feynman-learning-technique/?fbclid=IwAR2K5_BGPVo0QjJXkOIIqNsqcXK4lTskPWJvA0asKQIGtCPWaQBdKmj1Ztg), **without the help of Google:**

## General
* Why Python programming is awesome
* What is an object
* What is the difference between a class and an object or instance
* What is the difference between immutable object and mutable object
* What is a reference
* What is an assignment
* What is an alias
* How to know if two variables are identical
* How to know if two variables are linked to the same object
* How to display the variable identifier (which is the memory address in the CPython implementation)
* What is mutable and immutable
* What are the built-in mutable types
* What are the built-in immutable types
* How does Python pass variables to functions

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

## `.txt` Answer Files
* Only one line
* No Shebang
* All your files should end with a new line

# Tasks
Tasks table

| Task Name  | File Name | Description |
| --------------- | ------------------------------ |---------------------------------------------------------------|
| 0. Who am I? | `0-answer.txt` | A function would you use to print the type of an object |
| 1. Where are you? | `1-answer.txt` | How to get the variable identifier |
| 2. Right count | `2-answer.txt` | Does `a` and `b` point to the same object? |
| 3. Right count = | `3-answer.txt` | Does `a` and `b` point to the same object? |
| 4. Right count = | `4-answer.txt` | Does `a` and `b` point to the same object? |
| 5. Right count =+ | `5-answer.txt` | Does `a` and `b` point to the same object? |
| 6. Is equal | `6-answer.txt` | What do these 3 lines print? |
| 7. Is the same | `7-answer.txt` | What do these 3 lines print? |
| 8. Is really equal | `8-answer.txt` | What do these 3 lines print? |
| 9. Is really the same | `9-answer.txt` | What do these 3 lines print? |
| 10. And with a list, is it equal | `10-answer.txt` | What do these 3 lines print? |
| 11. And with a list, is it the same | `11-answer.txt` | What do these 3 lines print? |
| 12. And with a list, is it really equal| `12-answer.txt` | What do these 3 lines print? |
| 13. And with a list, is it really the same | `13-answer.txt` | What do these 3 lines print? |
| 14. List append | `14-answer.txt` | What does this script print? |
| 15. List add | `15-answer.txt` | What does this script print? |
| 16. Integer incrementation | `16-answer.txt` | What does this script print? |
| 17. List incrementation | `17-answer.txt` | What does this script print? |
| 18. List assignation | `18-answer.txt` | What does this script print? |
| 19. Copy a list object | `19-copy_list.py` | A function `def copy_list(l):` that returns a copy of a list |
| 20. Tuple or not? | `20-answer.txt` | Is `a` a tuple? |
| 21. Tuple or not? | `21-answer.txt` | Is `a` a tuple? |
| 22. Tuple or not? | `22-answer.txt` | Is `a` a tuple? |
| 23. Tuple or not? | `23-answer.txt` | Is `a` a tuple? |
| 24. Who I am? | `24-answer.txt` | What does this script print? |
| 25. Tuple or not | `25-answer.txt` | What does this script print? |
| 26. Empty is not empty | `26-answer.txt` | What does this script print? |
| 27. Still the same? | `27-answer.txt` | Will the last line of this script print `139926795932424`? |
| 28. Same or not? | `28-answer.txt` | Will the last line of this script print `139926795932424`? |
| 29. #pythonic | `100-magic_string.py` | A function `magic_string()` that returns a string `“BestSchool”` |
| 30. Low memory cost | `101-locked_class.py` | A class `LockedClass` with no class or object attribute |
| 31. int 1/3 | `103-line1.txt, 103-line2.txt` | CPython implementation of Python3 with default options/configuration |
| 32. int 2/3 | `104-line1.txt, 104-line2.txt, 104-line3.txt, 104-line4.txt, 104-line5.txt` | CPython implementation of Python3 with default options/configuration |
| 33. int 3/3 | `105-line1.txt` | CPython implementation of Python3 with default options/configuration |
| 34. Clear strings | `106-line1.txt, 106-line2.txt, 106-line3.txt, 106-line4.txt, 106-line5.txt` | CPython implementation of Python3 with default options/configuration |
