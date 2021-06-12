# Reading and Writing Files in Python 

### What Is a File?

At its core, a file is a contiguous set of bytes used to store data. This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable. In the end, these byte files are then translated into binary 1 and 0 for easier processing by the computer.

Files on most modern file systems are composed of three main parts:

- Header: metadata about the contents of the file (file name, size, type, and so on)

- Data: contents of the file as written by the creator or editor

- End of file (EOF): special character that indicates the end of the file

What this data represents depends on the format specification used, which is typically represented by an extension. For example, a file that has an extension of .gif most likely conforms to the Graphics Interchange Format specification.

### File Paths:

When you access a file on an operating system, a file path is required. The file path is a string that represents the location of a file. It’s broken up into three major parts:

Folder Path: the file folder location on the file system where subsequent folders are separated by a forward slash / (Unix) or backslash \ (Windows)
File Name: the actual name of the file
Extension: the end of the file path pre-pended with a period (.) used to indicate the file type.

Opening and Closing a File in Python:

When you want to work with a file, the first thing to do is to open it. This is done by invoking the _open()_ built-in function. _open()_ has a single required argument that is the path to the file. _open()_ has a single return, the file object:

```
file = open('dog_adventures.txt')

```

When you’re manipulating a file, there are two ways that you can use to ensure that a file is closed properly, even when encountering an error. The first way to close a file is to use the try-finally block:

```
reader = open('dog_adventures.txt')
try:
     # further file processing goes here
finally:
  reader.close()

  ```
  Prefered method:
  The second way to close a file is to use the with statement:

  ```
  with open('dog_adventures') as reader:
    # Further file processing goes here
    
  ```

  ### _mode_ is an optional string that specifies the mode in which the file is opened:
  
Character	Meaning:

- 'r'	Open for reading (default)

- 'w'	Open for writing, truncating (overwriting) the file first

- 'rb' or 'wb'	Open in binary mode (read/write using byte data)

  ### There are three different categories of file objects:

1. Text files
1. Buffered binary files
1. Raw binary files

[Reading and Writing Files in Python](https://realpython.com/read-write-files-python/)

# Python Exceptions: An Introduction

A Python program terminates as soon as it encounters an error. In Python, an error can be a syntax error or an exception.

_Syntax errors_ occur when the parser detects an incorrect statement.

 _Exception errors_ occurs whenever syntactically correct Python code results in an error.

 ### The AssertionError Exception:

Instead of waiting for a program to crash midway, you can also start by making an assertion in Python. We assert that a certain condition is met. If this condition turns out to be True, then that is excellent! The program can continue. If the condition turns out to be False, you can have the program throw an AssertionError exception.

### The try and except Block: Handling Exceptions:

The try and except block in Python is used to catch and handle exceptions. Python executes code following the try statement as a “normal” part of the program. The code that follows the except statement is the program’s response to any exceptions in the preceding try clause.

Here are the key takeaways:

A try clause is executed up until the point where the first exception is encountered.
Inside the except clause, or the exception handler, you determine how the program responds to the exception.
You can anticipate multiple exceptions and differentiate how the program should respond to them.
Avoid using bare except clauses.

### The else Clause:

In Python, using the else statement, you can instruct a program to execute a certain block of code only in the absence of exceptions.

### Cleaning Up After Using finally:

Imagine that you always had to implement some sort of action to clean up after executing your code. Python enables you to do so using the finally clause.

### Summing Up:

After seeing the difference between syntax errors and exceptions, you learned about various ways to raise, catch, and handle exceptions in Python. In this article, you saw the following options:

raise allows you to throw an exception at any time.
assert enables you to verify if a certain condition is met and throw an exception if it isn’t.
In the try clause, all statements are executed until an exception is encountered.
except is used to catch and handle the exception(s) that are encountered in the try clause.
else lets you code sections that should run only when no exceptions are encountered in the try clause.
finally enables you to execute sections of code that should always run, with or without any previously encountered exceptions.


[Python Exceptions: An Introduction](https://realpython.com/python-exceptions/)



 [<----- Back to About Me](../README.md)