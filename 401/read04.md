# File

**file** :is a contiguous set of bytes used to store data. This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable. In the end, these byte files are then translated into binary 1 and 0 for easier processing by the computer.

**Part of file**

1. Header: metadata about the contents of the file (file name, size, type, and so on)
2. Data: contents of the file as written by the creator or editor
3. End of file (EOF): special character that indicates the end of the file

![part](https://files.realpython.com/media/FileFormat.02335d06829d.png)

## File Paths
When you access a file on an operating system, a file path is required. The file path is a string that represents the location of a file. It’s broken up into three major parts:

1. Folder Path: the file folder location on the file system where subsequent folders are separated by a forward slash / (Unix) or backslash \ (Windows)
2. File Name: the actual name of the file
3. Extension: the end of the file path pre-pended with a period (.) used to indicate the file type

## Opening and Closing a File in Python

* open a file 

``` 
file = open('file_name.extension') 
```

It’s important to remember that it’s your responsibility to close the file. In most cases, upon termination of an application or script, a file will be closed eventually. However, there is no guarantee when exactly that will happen. This can lead to unwanted behavior including resource leaks. It’s also a best practice within Python (Pythonic) to make sure that your code behaves in a way that is well defined and reduces any unwanted behavior.

* close a file
1. finaly block
```
reader = open('file_name.extension')
try:
    # Further file processing goes here
finally:
    reader.close()
```

2.  with statement

```
with open('file_name.extension') as reader:
    # Further file processing goes here
 ```   

 **you can put inside open second parameter >>
  second positional argument, mode. This argument is a string that contains multiple characters to represent how you want to open the file. The default and most common is 'r', which represents opening the file in read-only mode as a text file**


  

|Character|	Meaning|
|------|------|
|'r'|	Open for reading (default)|
|'w'|	Open for writing, truncating (overwriting) the file first|
|'rb' or 'wb'|	Open in binary mode (read/write using byte data)|

----

## There are three different categories of file objects:

* Text files
* Buffered binary files
* Raw binary files

-----
* text file 
1. how to open it
```
open('abc.txt')
open('abc.txt', 'r')
open('abc.txt', 'w')
```


2.  **open() will return a TextIOWrapper file object**
 ```
 >>> file = open('dog_breeds.txt')
>>> type(file)
<class '_io.TextIOWrapper'>
 ```

 * Buffered Binary File Types

 1. how to open it
 ```
open('abc.txt', 'rb')
open('abc.txt', 'wb')
 ```

2.  open() will return either a BufferedReader or BufferedWriter file object
```
>>> file = open('dog_breeds.txt', 'rb')
>>> type(file)
<class '_io.BufferedReader'>
>>> file = open('dog_breeds.txt', 'wb')
>>> type(file)
<class '_io.BufferedWriter'>
```

* Raw File Types (generally used as a low-level building-block for binary and text streams)
1. how to open it

```
open('abc.txt', 'rb', buffering=0)
```

2. open() will return a FileIO file object

```
>>> file = open('dog_breeds.txt', 'rb', buffering=0)
>>> type(file)
<class '_io.FileIO'>
```

## Reading and Writing Opened Files

|Method	|What It Does| 
|------|------------|
|.read(size=-1)|	This reads from the file based on the number of size bytes. If no argument is passed or None or -1 is passed, then the entire file is read.|
|.readline(size=-1)|	This reads at most size number of characters from the line. This continues to the end of the line and then wraps back around. If no argument is passed or None or -1 is passed, then the entire line (or rest of the line) is read.|
|.readlines()	|This reads the remaining lines from the file object and returns them as a list.|

**we can use list(f) instead of f.readlines()**

## writing files


|Method	|What It Does|
|---|---|
|.write(string)	|This writes the string to the file.|
|.writelines(seq)	|This writes the sequence to the file. No line endings are appended to each sequence item. It’s up to you to add the appropriate line ending(s).|



# Python Exceptions: An Introduction

## Exceptions versus Syntax Errors

**Syntax errors occur when the parser detects an incorrect statement. Observe the following example:**

```
>>> print( 0 / 0 ))
  File "<stdin>", line 1
    print( 0 / 0 ))
                  ^
SyntaxError: invalid syntax
```
**The arrow indicates where the parser ran into the syntax error. In this example, there was one bracket too many. Remove it and run your code again:**

```
>>> print( 0 / 0)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
ZeroDivisionError: integer division or modulo by zero
```

This time, you ran into an exception error. This type of error occurs whenever syntactically correct Python code results in an error. The last line of the message indicated what type of exception error you ran into.

Instead of showing the message exception error, Python details what type of exception error was encountered. In this case, it was a ZeroDivisionError.

## Raising an Exception

```
x = 10
if x > 5:
    raise Exception('x should not exceed 5. The value of x was: {}'.format(x))
```

```
Traceback (most recent call last):
  File "<input>", line 4, in <module>
Exception: x should not exceed 5. The value of x was: 10
```

## The AssertionError Exception
```
import sys
assert ('linux' in sys.platform), "This code runs on Linux only."
```

```
Traceback (most recent call last):
  File "<input>", line 2, in <module>
AssertionError: This code runs on Linux only.
```

## The try and except Block: Handling Exceptions
![image](https://files.realpython.com/media/try_except.c94eabed2c59.png)


## The else Clause
![image](https://files.realpython.com/media/try_except_else.703aaeeb63d3.png)

## Cleaning Up After Using finally

![image](https://files.realpython.com/media/try_except_else_finally.a7fac6c36c55.png)

# things I need to know more about



# Refrences
1. Real Python. (2022, September 23). Reading and Writing Files in Python (Guide). Retrieved October 8, 2022, from [link](https://realpython.com/read-write-files-python/)
2. Real Python. (2022, September 23). Reading and Writing Files in Python (Guide). Retrieved October 8, 2022, from [link](https://realpython.com/read-write-files-python/)