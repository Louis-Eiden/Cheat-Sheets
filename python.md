# Python Cheatsheet

---

## **UNDER CONSTRUCTION**

---

## Table of Contents

- [Introduction](#introduction)
- [Variables](#variables)
- [Data Types](#data-types)
- [Control Flow](#control-flow)
- [Functions](#functions)
- [Modules](#modules)
- [File Handling](#file-handling)
- [Exception Handling](#exception-handling)
- [Classes and Objects](#classes-and-objects)
- [Regular Expressions](#regular-expressions)
- [Debugging](#debugging)
- [Additional Resources](#additional-resources)
- [Commands](#commands)
- [Syntax](#syntax)
- [Examples](#examples)

## Python Installation

https://www.python.org/downloads/

https://www.infoworld.com/article/3530140/how-to-install-python-the-smart-way.html#:~:text=By%20default%20the%20Python%20installer,directory%20(e.g.%20C%3A%5CPython3.

https://www.youtube.com/watch?v=i-MuSAwgwCU&t=77s

install python with apt:

> sudo apt update
> sudo apt install python3

verify python installation:

> python3 --version

create a symlink for python3:

> sudo ln -s /usr/bin/python3 /usr/bin/python

install pip:

> sudo apt install python3-pip

## Virtual Environment

> python -m venv venv

activate virtual environment:

> source venv/bin/activate

deactivate virtual environment:

> deactivate

## Introduction

- Python is a high-level programming language...
- ...

## Variables

- Declaring variables
- Variable naming conventions
- ...

## Data Types

- Numeric types (int, float, complex)
- String type
- List, tuple, and set types
- ...

## Control Flow

- if-else statements
- for and while loops
- break and continue statements
- ...

## Functions

- Defining and calling functions
- Function arguments and return values
- Lambda functions
- ...

## Modules

- Importing modules
- Using built-in modules
- Creating and using custom modules
- ...

## File Handling

- Opening and closing files
- Reading and writing files
- File modes and file objects
- ...

## Exception Handling

- Handling exceptions with try-except blocks
- Raising exceptions
- ...

## Classes and Objects

- Defining classes and creating objects
- Class attributes and methods
- Inheritance and polymorphism
- ...

## Regular Expressions

- Pattern matching with regular expressions
- Using regex functions and methods
- ...

## Debugging

- Using print statements
- Debugging with breakpoints
- ...

## Additional Resources

- Online tutorials and documentation
- Python community and forums
- ...

## Commands

Here are some useful commands for Python:

- `python`: Run a Python script or start the Python interpreter.
- `pip`: Install Python packages from the Python Package Index (PyPI).
- `virtualenv`: Create isolated Python environments.
- `pylint`: Check Python code for errors and style issues.
- `pytest`: Run Python unit tests.
- `pdb`: Python debugger for interactive debugging.
- `python -m venv`: Create a virtual environment.
- `python -m http.server`: Start a simple HTTP server.
- `python -m json.tool`: Format JSON data.
- `python -m timeit`: Measure execution time of small bits of Python code.
- `python -m doctest`: Test interactive Python examples in docstrings.
- `python -m unittest`: Run unit tests in a module or directory.
- `python -m pip install`: Install Python packages.
- `python -m pip uninstall`: Uninstall Python packages.
- `python -m pip freeze`: Output installed Python packages in requirements format.
- `python -m pip list`: List installed Python packages.
- `python -m pip show`: Show information about an installed Python package.
- `python -m pip search`: Search PyPI for Python packages.
- `python -m pip check`: Verify installed Python packages have compatible dependencies.
- `python -m pip upgrade`: Upgrade installed Python packages.
- `python -m pip install --upgrade pip`: Upgrade pip itself.
- `python -m ensurepip`: Install or upgrade pip and other Python packaging tools.
- `python -m site`: Show information about the Python site module.
- `python -m compileall`: Byte-compile Python source files.
- `python -m pydoc`: Start the Python documentation server.
- `python -m trace`: Trace Python program execution.
- `python -m tokenize`: Tokenize Python source code.
- `python -m tabnanny`: Detect inconsistent use of tabs and spaces in Python source code.
- `python -m py_compile`: Compile Python source files to bytecode.
- `python -m runpy`: Locate and run Python modules.
- `python -m ensurepip --upgrade`: Upgrade pip and other Python packaging tools.
- `python -m ensurepip --user`: Install or upgrade pip and other Python packaging tools for the current user.
- `python -m ensurepip --upgrade --user`: Upgrade pip and other Python packaging tools for the current user.

## Syntax

Here are some important syntax rules in Python:

- Indentation: Python uses indentation to define blocks of code. Use 4 spaces or a tab for each level of indentation.
- Comments: Use the `#` symbol to add comments in your code. Comments are ignored by the interpreter.
- Variables: Variables are created when you assign a value to them. No need to declare the type explicitly.
- Strings: Strings can be enclosed in single quotes (`'`) or double quotes (`"`). Use the `+` operator to concatenate strings.
- Lists: Lists are ordered, mutable collections of items. Use square brackets (`[]`) to define a list.
- Tuples: Tuples are ordered, immutable collections of items. Use parentheses (`()`) to define a tuple.
- Dictionaries: Dictionaries are unordered collections of key-value pairs. Use curly braces (`{}`) to define a dictionary.
- Control Flow: Use if-else statements, for and while loops, and break and continue statements to control the flow of your program.
- Functions: Use the `def` keyword to define functions. Functions can have arguments and return values.
- Classes: Use the `class` keyword to define classes. Classes can have attributes and methods.
- Exception Handling: Use try-except blocks to handle exceptions and prevent your program from crashing.
- Importing Modules: Use the `import` keyword to import modules and use their functionality in your code.

## Examples

Here are some examples to illustrate Python concepts:

- Example 1: Declaring and using variables
